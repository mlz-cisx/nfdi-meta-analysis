# The Photon and Neutron Open Science Cloud (PaNOSC)
##### tags: `#TA2` `#TA3`
https://www.panosc.eu/deliverables/
PaNOSC is a European project for making FAIR data a reality in 6 European Research Infrastructures (RIs), developing and providing services for scientific data and connecting these to the European Open Science Cloud (EOSC).


## Common Search API
https://www.panosc.eu/deliverables/deliverable-3-1-api-definition-common-search-api/
D3.1 marks the delivery of the first version of a common search API (Application Programming Interface) for open data. This API will be implemented by all PaNOSC partner sites and ExPaNDS and any further facilities that want to join this effort as part of the EOSC. This search API allows to find datasets and data publications based on relevant domain specific metadata and can be used by third parties to find data that has been released from any facility-imposed embargo period, as well as by the original researchers. This will be an important entry point for anyone to use the EOSC visualisation, processing or data transfer services that are being developed in other PaNOSC Work Packages. 

The common search API is standardized to the outside. It needs to be implemented seperately for every metadata catalogue however.

- https://indico.esss.lu.se/event/1373/contributions/10464/attachments/9757/15633/2020-02-11_harvesting.pdf
- Uses Loopback and its search filter

## Federated Search API
https://www.panosc.eu/wp-content/uploads/2021/11/PaNOSC_D3.2_DemonstratorImplementation_20210324.pdf
This document summarises the development of a federated search demonstrator created in the PaNOSC Work Package 3. It explains the development and many of the decisions made, as well as open tasks for future development.

The federated search is the gateway for all data search requests. It calls the common searc API of every institutes, aggregates the results and returns them to the requester.

- Uses Loopback and its search filter
- Could be replaced with OpenAIRE Connect
- Federated search enables automatic search for data to use in other services: federated search -> data transfer -> data analysis

![](https://iffmd.fz-juelich.de/uploads/upload_d6c7c5c9642ea38b133d3c12c6179dc2.png)


## Harvesting API
https://github.com/panosc-eu/harvest-api
- For Websites like OpenAIRE to harvest data from it
- Currently uses the OAI-PMH protocol

Harvesting is a process done by other repository registries. They copy the provided metadata and make it available on their website, along with a link to the original source. For more information on repository registries, go to the dedicated section further down below.


## Data Catalogue
https://www.panosc.eu/services/data-catalogue/
This document marks the delivery of a federated domain specific search as a service for open data from PaN RIs. The search API service is running and serves live data from PaNOSC and ExPaNDS partner sites (ESRF, ESS, ILL and MaxIV). There is even a user web frontend that has been created in collaboration with WP4. 

The work builds on the two previous deliverables of PaNOSC WP3. First the API was proposed. In the second iteration the API was improved with input from the proof-of-concept demonstrator and site installations. Deploying the search API as a service for the community as part of this deliverable led to a number of improvements and clarifications in the API, driven by the practical use. In addition, the earlier API definitions left the question of how datasets can be queried using the techniques ontology and how to rank (score) results from different facilities open. This has now been defined and the implementation of the relevant modules at the partner sites has started. 

- Panos uses b2find, which is a service by EOS: https://b2find.eudat.eu/group/panosc

## Software Catalogue
https://www.panosc.eu/services/pan-software-catalogue/

## Data Analysis
https://www.panosc.eu/services/data-analysis/
- The tool is called VISA
- Heavy (uses openstack) but many features

## Data Simulation (JupyterHub)
https://www.panosc.eu/services/data-analysis-simulation-data-system/