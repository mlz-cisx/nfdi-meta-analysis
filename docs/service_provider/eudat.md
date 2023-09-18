# EUDAT
##### tags: `#PIs` `#TA3`
https://sp.eudat.eu/catalogue/

The EUDAT Collaborative Data Infrastructure (or EUDAT CDI) is one of the largest infrastructures of integrated data services and resources supporting research in Europe. It is sustained by a network of more than 20 European research organisations, data and computing centres that on September 2016 have signed an agreement to maintain the EUDAT CDI for the next 10 years and in 2018 have supported the establishment of the limited liability company, EUDAT Ltd.

This infrastructure and its services have been developed in close collaboration with over 50 research communities spanning across many different scientific disciplines and involved at all stage of the design process.

<br>

## B2Find
B2FIND is an interdisciplinary  discovery portal for research output that allows free term search, results may be narrowed down using several facets, including spatial and temporal search options.

B2FIND is the EUDAT metadata indexing service and provides a discovery portal which allows users to find data collections within an international and inter-disciplinary scope. It is based on a comprehensive metadata catalogue of research data collections stored in EUDAT data centres and community repositories. Harmonization of the metadata descriptions collected from heterogeneous sources enables not only the presentation in a consistent form but as well the faceted search across scientific domain boundaries. For Communities and other providers of research data who need to publish and give visibility to their metadata and individual researchers who need to search data from everywhere, and see data in the context with an across community approach.

Features:
- Harmonization of the metadata descriptions via the EUDAT Core metadata schema
- Harvesting of repositories via different protocols (e.g. OAI-PMH, CSW, Rest-APIs)
- Facetted search via 17 facets (including geospatial, temporal search options), additional free text search
- Metadata aggregation from community repositories, multiple metadata standards are supported
- Harvested by OpenAIRE explorer


<br>

## B2Safe
B2SAFE is a robust and highly available service which allows community and departmental repositories to implement data management policies on their research data across multiple administrative domains in a trustworthy manner. It offers an abstraction layer of large scale, heterogeneous data storages, guards against data loss in long-term archiving, allows to optimize access for users (e.g. from different regions), brings data closer to facilities for compute-intensive analysis.

Features:
- Support for data management policies (e.g. registration of PIDs, cross-site replication, data integrity checks)
- Support for policies customised to community and organisational needs
- Support for less frequently used archival data, but can also support active data
- Support for large scale storage resources (e.g up to PB-scale)
- A single namespace across hetrogeneous storages
- Supports integration with different kind of storage systems (e.g. Tape based HSM, POSIX filesystems, Object storage)
- Access via GridFTP, Webdav, iRODS commands
- Service offered by a network of EUDAT service providers


<br>

## B2Share
B2SHARE is a user-friendly, reliable and trustworthy way for researchers, scientific communities and citizen scientists to store, publish and share research data in a FAIR way. B2SHARE is a solution that facilitates research data storage, guarantees long-term persistence of data and allows data, results or ideas to be shared worldwide. B2SHARE supports community domains with metadata extensions, access rules and publishing workflows. EUDAT offers communities and organisations customised instances and/or access to repositories supporting large datasets.

Features: 
- Support of metadata descriptions via the EUDAT metadata schema
- Registers DOIs for datasets and Handle PIDs for data objects
- Supports versioning
- Harvested by B2FIND and OpenAIRE explorer
- Direct upload from B2DROP
- Accessible via a Web GUI and an API to support automatic publishing workflows
- Supports community domains
- Allows communities to define metadata extensions, access rules and publishing workflows


<br>

## B2Drop
B2DROP is a low-barrier, user-friendly and trustworthy storage environment which allows users to synchronise their active data across different desktops and to easily share this data with peers. EUDAT offers a free public basic instance for any researcher. For communities and organisations a premium service is offered on the public instance. Communities and organisations can also request customised instances.

Features:
- Default quota of 20GBs (Basic), high quotas optional (Premium)
- Access via Web GUI, desktop clients and Webdav
- Multiple versions of files are kept
- Enabled apps: Contacts, Calendar, Tasks, Circles (social communities)
- Sharing within B2DROP, across different instances (via OCM-API) and via links
- Publishing of datasets to B2SHARE
- Integration with CLARIN Language Resource Switchboard (Basic)
- Integration with other community services optional (Premium)
- Group management (Premium)
- OnlyOffice (Premium)


<br>

## B2Note
B2NOTE allows to easily create, search and manage annotations. An annotation is a keyword or commentary attached to a data object (data collection, file) that explains or classifies it. B2NOTE is a central service for annotating data content hosted within the EUDAT CDI.

B2NOTE supports 3 types of annotations:
- the semantic tag, a keyword from an ontology (a semantic tag coming from identified ontology repositories - currently only Bioportal
- the free-text keyword, to be created and used when a specific semantic term is not found
- the comment, a more comprehensive annotation

Relevant for:
- User must register to create and maintain annotations, additional access registration can be applied on the service which enabled annotation functionality via B2NOTE.
- Service providers willing to enable annotation via B2NOTE on an existing service can request consultancy and support

Features:
- Is integrated into B2SHARE: access data via B2SHARE, then annotate them with B2NOTE
- Annotations are created and stored in a computer-readable format using the W3C Web Annotation model
- Annotations are searchable (in opposite to hand-written annotations). 
- Search results can be visualized in the User Interface and refined before being exported either as JSON-LD for reuse with your analysis workflow/script/software. 
- Allows users to export all the annotations about a file as JSON-LD for your own purpose. 
- This version is a crowdsourcing annotation service meaning that all annotations will be publicly available. To preserve the anonymity as a user you can register and create an annotator pseudonym.


<br>

## B2Access
B2ACCESS is a federated cross-infrastructure authorisation and authentication proxy for user identification and community-defined access control enforcement. It allows users to authenticate themselves using a variety of credentials providing federated access and single-sign-on to services and service providers in a trusted way. B2ACCESS offers communities and service providers an AARC compliant AAI proxy ready to be integrated within the EOSC AAI Federation.

Features:
- Compliant to the AARC Blueprint and REFEDS Sirtfi
- Supports group management
- Supports authorisation via group membership
- Supports authentication e.g. via eduGAIN, ORCID and Social Identities
- Support for EUDAT B2ACCESS local accounts
- Support for IdP and service integration via SAML, OAuth and OIDC


<br>

## B2Handle
B2HANDLE is the distributed service for storing, managing and accessing persistent identifiers (PIDs) and essential metadata (PID records) as well as managing PID namespaces. The implementation of the service relies on the DONA/Handle persistent identifier solution. B2HANDLE can be used by middleware applications, end-user tools and other service to reliably identify data objects over longer timespans and through changes in object location or ownership. The B2HANDLE service encompasses management of identifier namespaces (Handle prefixes), establishment of policies and business workflows, operation of Handle servers and technical services, and a user-friendly Python library for general interaction with Handle servers and EUDAT-specific extensions. B2HANDLE is mostly transparent to end-users, shielding them from the complexity of infrastructure details. B2HANDLE supports a dedicated Handle record structure (a PID profile) for the safe data management within an infrastructure with a given topology.

Features:
- Globally resolvable identifiers via the Global Handle Network (DONA, https://hdl.handle.net/)
- Communities and organisations can obtain Handle Prefixes (ePIC, 21.####) for their own use
- PIDs can be hosted at EUDAT service providers
- B2HANDLE operates as a federation of EUDAT service providers based on policies
- PIDs are mirrored across multiple providers for high resolution and high availability
- Handle records can be customised to community and organisational needs (for example include checksums and timestamps to ensure authenticity of the data objects)
- Support for reverse look-ups of Handle records
- REST API for easy registration and minting of PIDs