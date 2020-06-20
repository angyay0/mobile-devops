# Welcome
This file contains examples to create CI experiences for iOS target.

The first task is upload our iOS repository if we want to keep track inside Azure DevOps, but we can use other sources instead.

## Continuous Integration
The first thing is connecting the repo, we can choose from different sources.
!["Repo Connection"](img/00.PNG)

The prebuilt template for iOS contains all the required steps to generate a non-signed bundle to deploy in simulator.
!["Task Template"](img/01.PNG)

The agent for running the pipeline choose mac distribution.
!["Agent Configuration"](img/02.PNG)

For generate a signed apk, we must provision the p12 certificate file and provisioning profile for signing the build.
!["Signing Configuration"](img/03.PNG)
!["Signing Configuration"](img/04.PNG)


Last step is save and queue pipeline

!["Save Pipeline"](img/05.PNG)


## Continuous Delivery
Currently exist some steps, but for integrating with Official Stores we highly recommend working with AppCenter CD.
