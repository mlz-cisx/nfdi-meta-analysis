# REANA
##### tags: `#TA2` `#TA3`

Created by **PUNCH4NFDI**

[REANA](https://www.reana.io/) is a reproducible analysis platform allowing scientists to run containerised data analysis pipelines on remote compute clouds.

The analysis is structured based on four questions: (i) where is the input data and parameters, (ii) what code is used to analyse the data, (iii) which computing environments are used to run the analysis code, and (iv) what are the computational steps taken to arrive at the results.

REANA supports several declarative workflow systems (CWL, Snakemake, Yadage), parses the workflow specification described by the researcher and dispatches its computational steps to several supported compute backends (Kubernetes, HTCondor, Slurm). The reproducibility of computations is assisted by means of using software containers (Docker, Singularity) that fully encapsulate the computational environment.

Thanks to the declarative programming approach and the support for multiple workflow engines and multiple compute backends, REANA also allows using hybrid computational workflow paradigm where parts of the analysis is run on one compute backend whilst the other parts of the analysis are seamlessly dispatched to other compute backend based on high-throughput or high-performance computing needs of the step at hand.