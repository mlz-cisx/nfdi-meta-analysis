# VISA
##### tags: `TA3`

Documentation: https://visa.readthedocs.io/en/latest/

Overview: https://www.panosc.eu/services/data-analysis/

VISA (Virtual Infrastructure for Scientific Analysis) is a platform that makes it simple to create compute instances on an OpenStack infrastructure to enable scientific users to analyse their experimental data remotely using just a web browser.

## Architecture
The control software is based on container technologies and is deployed via kubernetes, while the analysis environment is managed via VMs. Because of this, OpenStack is a prerequisite.