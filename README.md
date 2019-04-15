[![Build Status](https://travis-ci.org/HegemanLab/galomix.svg?branch=master)](https://travis-ci.org/HegemanLab/galomix)

# galomix

Galomix is a lab appliance for running [Galaxy severs](https://github.com/galaxyproject/galaxy).

Included with Galomix are Galaxy configurations for running a metabolomics lab appliance.

## Container Management

[Usernetes](https://github.com/rootless-containers/usernetes) is Galomix' default container management system. Kubernetes can be used instead. The advantage of Usernetes is that it can run containers without root privilege. An [overview of Usernetes](https://fosdem.org/2019/schedule/event/containers_k8s_rootless/) was presented at FOSDEM 2019.
