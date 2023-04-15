# Design Documentation
Initial design and documentation of Archura Router.

The `01 - Archura Filters and Standard Apps - High Level Diagrams.drawio.xml` 
file contains the high level diagrams for the Archura Router. 

You can open it with [draw.io](https://www.draw.io/).


## -Initialization
* Load configuration (file/remote)
* (Optional) Connect to Notification
* (Optional) Populate Cache

## Filters
Most of these filters can be configured as global or specific filters. 
Most filters can be configured for domain, tenant, user or route.

* [G]-Logging
* [G]-Tracing
* [G]-Monitoring

* [G]-Domain (D: Domain)
* [D]-Tenant (T: Tenant)

* [G]-Header (Create/Add Domain Token)
* [G]-BlackWhiteListing for Domain
* [G]-Throttling for Domain  (request size/time)
* [G]-Rate Limiting for Domain (# of requests/time)

* [D/T]-Route matching (+A/B)
* [D/T]-Authentication
* [D/T]-Authorization
* [D/T]-RevokeAccess
* [D/T]-Auditing
* [D/T]-Throttling (Domain/Tenant/User)
* [D/T]-Rate Limiting (Domain/Tenant/User)
* [D/T]-Header (validate, add/remove)
* [D/T]-Caching
* [D/T]-Webhook (async)
* [D/T]-Predefined Response
* [D/T]-Timeout
* [D/T]-Retry
* [D/T]-WeightedRoundRobin
* [D/T]-Parallelization
* [D/T]-CircuitBreaker
* [D/T]-ExternalHttpFilter

* [G]-Routing
  - Domain / Customer Account
  - Tenant
  - RouteId
  - Router-Token (Domain cert.)
  - Request: Method/Headers/Body

... Post Filters


