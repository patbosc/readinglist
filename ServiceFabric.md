Service Fabric
---------

Getting Started
--

Okay basically Service Fabric is one of the coolest technologies I ever had the pleasure working with. However the correct setup of a cluster and running the infrastructure sometimes is crazy. People have great ideas how not to use it. 

- [Service Fabric Architecture Overview MSFT](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-architecture?WT.mc_id=personal-blog-marouill)
- [Service Fabric Terminology Overview](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-content-roadmap?WT.mc_id=personal-blog-marouill)
- [Working with Certificates in Microsoft Azure Getting Started](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-create-cluster-using-cert-cn)
- [Certificates Overview in Service Fabric](https://docs.microsoft.com/en-us/azure/service-fabric/cluster-security-certificate-management)
- [Cluster Security](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-cluster-security)
- [Security Best Practices](https://docs.microsoft.com/en-us/azure/security/fundamentals/service-fabric-best-practices)
- [Configure Standalone Cluster](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-cluster-manifest)
- Cluster [networking patterns internal/external load balancer](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-patterns-networking)

- [durability tier explained](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-cluster-capacity).
- [Azure Scalset SLA](https://azure.microsoft.com/en-us/support/legal/sla/virtual-machines/v1_9/)
- [availability zones](https://docs.microsoft.com/en-us/azure/availability-zones/az-overview)

See [scalability concepts](https://github.com/MicrosoftDocs/azure-docs/blob/master/articles/service-fabric/service-fabric-concepts-scalability.md) and [scale a sf cluster in azure](https://github.com/MicrosoftDocs/azure-docs/blob/master/articles/service-fabric/service-fabric-tutorial-scale-cluster.md) for more details.

- [Additional Service Fabric Cluster Templates ARM](https://github.com/Azure-Samples/service-fabric-cluster-templates)

Cluster Planning
---
- [Capacity Planning](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-capacity-planning)
- [Fault Analysis Services](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-testability-overview)

- Tools for cluster planning:

Use profilers like [ANTS](https://www.red-gate.com/products/dotnet-development/ants-memory-profiler/), [dotMemory](https://www.jetbrains.com/dotmemory/?gclid=Cj0KCQjw6NmHBhD2ARIsAI3hrM1MqFcSB8oY_P0AUoFzzx5F2WPiAQm0c4mJGuO2Y81IxK7P7GhiNUYaAsJXEALw_wcB) or [Visual Studio Diagnostics Tools](https://docs.microsoft.com/en-us/visualstudio/profiling/memory-usage-without-debugging2?view=vs-2019). Running a local or cloud based [LoadTest](https://docs.microsoft.com/en-us/visualstudio/test/walkthrough-create-and-run-a-load-test?view=vs-2019)

Documentation
---
- [Overview](https://docs.microsoft.com/en-us/azure/service-fabric/service-fabric-overview)

Microsoft Virtual Academy:
---
- [Building Microservices Applications on Azure Service Fabric](https://mva.microsoft.com/en-US/training-courses/building-microservices-applications-on-azure-service-fabric-16747?l=HhD9566yC_4106218965)

Help & Support with Limits and Quotas
---

There are several Limits and Quotas which may or may not be increased. Check out the service [limits documentation](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/azure-subscription-service-limits). 

> Please note VM Scaleset need often more instances of a particular VM-Type. However the default quotas per vm-type is 10. Basic Guidence how to increase quota: [Increase VM series vCPU limit.](https://docs.microsoft.com/en-us/azure/azure-portal/supportability/per-vm-quota-requests)

> Increase Ingess Quota. This is the official how to guide on [increase ingress quota.](https://docs.microsoft.com/en-us/azure/azure-portal/supportability/networking-quota-requests)

### Networking Quotas

| Resource  | Target  |
|---|---|
| Virtual networks   | 	1,000 |
| Subnets per virtual network  | 	3,000 |
| Virtual network peerings per virtual network   | 	500 |
| [Virtual network gateways (VPN gateways) per virtual network](https://docs.microsoft.com/en-us/azure/vpn-gateway/vpn-gateway-about-vpngateways#gwsku)   | 1 |
| [Virtual network gateways (ExpressRoute gateways) per virtual network](https://docs.microsoft.com/en-us/azure/expressroute/expressroute-about-virtual-network-gateways#gwsku)   | 1 |

> Github [Azure VNET Limits Overview](https://github.com/MicrosoftDocs/azure-docs/blob/master/includes/azure-virtual-network-limits.md)

> See more Official Documentation [Network limits can be found here](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/azure-subscription-service-limits#networking-limits)

> Increase Ingess Quota. This is the how to guide how to [increase ingress quota.](https://docs.microsoft.com/en-us/azure/azure-portal/supportability/networking-quota-requests) 

> See [SLA for VPN Gateway](https://azure.microsoft.com/en-us/support/legal/sla/vpn-gateway/v1_4/)

### Application Gateway Quota

Application Gateway is part of [the networking quotas and limits](https://docs.microsoft.com/en-us/azure/azure-resource-manager/management/azure-subscription-service-limits#networking-limits).

 Resource  | Target  |
|---|---|
| Front-end IP configurations   | 	2 |
| Front-end ports   | 40 |
| Back-end address pools   | 40 |
| Front-end IP configurations   | 	2 |
| HTTP listeners  | 40 |

> In case of WAF-enabled SKUs, you must limit the number of resources to 40.
Sometimes the Limit is per Application Gateway instance not per Application Gateway resource.

