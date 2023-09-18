# Rucio

## Description

[Rucio](https://rucio.cern.ch/) is an open-source software framework that provides scientific collaborations with the functionality to organize, manage, and access their data at scale. The data can be distributed across heterogeneous data centers at widely distributed locations. Rucio was originally developed to meet the requirements of the high-energy physics experiment ATLAS, and now is continuously extended to support the LHC experiments and other diverse scientific communities. In this article, we detail the fundamental concepts of Rucio, describe the architecture along with implementation details, and report operational experience from production usage.

## Policy-Driven
Declarative data management allows you to say what you want, and let Rucio figure out the details how to do it. Manage your data with expressive statements. Three copies of my file on different continents, and have one backup on tape? Automatically remove it once its access popularity goes to zero? No problem.

## Features
- Namespaces
- Storage Support (Tape, cloud, supercomputer, ...)
- Authentication and Authorisation
- Monitoring (Graphite, ElasticSearch, Hadoop)
- Data Recovery Mechanisms
