# NOMAD
##### tags: `#TA2` `#TA3`

- https://fairmat-nfdi.eu/nomad-lab
- [Documentation](https://nomad-lab.eu/prod/v1/docs/)

Storage (Raw) -> Archive (Processed), AI Toolkit

The NOMAD web-application (formaly known as the NOMAD Repository and Archive) allows you to publish materials science research data.
It enables the confirmatory analysis of materials data, their reuse, and repurposing. All data is available in their original raw format, e.g. as produced by an underlying simulation code, (Repository) and in a common, machine-processable, and well-defined data format (Archive). Data can be downloaded and used under the CC-BY-4.0 license.
Data can be uploaded without any barrier: results are accepted as they are; only author information and optional comments or references must be provided. We allow private curation of data before publishing; data can be published with a 3-year embargo and selectively shared. You can request digital objective identifiers (DOI's) for your datasets and cite your data.

## Workflow
- Input generation: pymatgen
- Error correction: Custodian
- Workflow execution: FireWorks
- Data storage: mongoDB
- Data analysis: pymatgen


### FireWorks
- General purpose workflow manager
- Automate calculations over arbitrary computing resources
- Support for several queueing systems (PBS, SLURM, ...)
- Clean & flexible Python API
- Centralized database of jobs (MongoDB) + Workers
- Support for dynamic workflows
- Web gui monitor


##  NOMAD Metainfo

The NOMAD Metainfo can be understood as the schema of the NOMAD Archive. The NOMAD Archive data is structured to be independent of the electronic-structure theory code or molecular-simulation, (or beyond). The NOMAD Metainfo can be browsed as part of the NOMAD Repository and Archive web application.

Typically, (meta-)data definitions are generated only for a predesigned and specific scientific field, application, or code. In contrast, the NOMAD Metainfo considers all pertinent information in the input and output files of the supported electronic-structure theory, quantum-chemistry, and molecular-dynamics (force-field) codes. This ensures complete coverage of all material and molecule properties, even though some properties might not be as important as others, or are missing in some input/output files of electronic-structure programs.


##  NOMAD Oasis

[NOMAD Oasis](https://fairmat-nfdi.eu/nomad-lab/services-nomad-lab/oasis-nomad-lab) allows you to benefit from NOMAD's data management features within the premises of your organisation. Before you publish data on NOMAD, manage your data in your Oasis!

NOMAD and NOMAD Oasis are the same software operated at different places. Install NOMAD on a server in your institute and start managing your data.


## Upcoming
- ELN
- neXus & HDF5
- NORTH


### NORTH
The NOmad Remote Tools Hub allows to run containarized tools directly on the server. All you data will be mounted into the tool's container and you can read and write your data with tools like JupyterLab. You can extend the availble tools for your Oasis.