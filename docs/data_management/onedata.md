# Onedata
##### tags `TA3`

https://onedata.org

High-performance data management solution that offers unified data access across globally distributed environments and multiple types of underlying storage, allowing users to share, collaborate and perform computations on the stored data easily.


## Spaces
All data stored in Onedata is organized into Spaces. Spaces can be seen as virtual directories or volumes, which can contain an arbitrary directory and file hierarchy, while being distributed across multiple storage providers.


## Providers
Each zone is composed of a network of providers who provision their storage resources to users. Anyone can become a Onedata provider by installing Oneprovider service, attaching storage resources and registering it in a particular Onezone service.


## Zones
Onedata is a distributed system divided into zones that are created by deploying a dedicated service called Onezone. Any organization, community or user group can deploy their own Onezone service with customized login page and either connect it to the distributed network of Onezone services or run it as an isolated private deployment.

Onezone is responsible for authentication and authorization of users and makes it possible for users from different zones to communicate with each other and share data. It allows providers from different zones to interact with each other, i.e., allowing users from different zones to get support for their spaces regardless of the zone in which the particular provider is located.