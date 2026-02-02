# Home Assistant install using ArgoCD


## Directory layout
Every directory at the base level contains one application. So the Home Assistant Core manifests resides in the home-assistant directory, ESPHome resides in esphome, etcetera. Within every directory there is at least a deployments directory. This directory contains at least one target platform, for example production or development. If the target is development, there is another directory in there, which can be given the branch name of the feature under development.
Within every target directory there is a yaml file that describes what needs to be deployed. This can be a helm-chart, either localy stored or from a repository. The first one is called helm-source.yaml and can be kept empty. The second one, is called helm-application.yaml and needs to 
