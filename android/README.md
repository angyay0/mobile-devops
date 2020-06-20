# Welcome
This file contains examples to create CI experiences for Android target.

The first task is upload our android repository if we want to keep track inside Azure DevOps, but we can use other sources instead.

## Continuous Integration
The first thing is connecting the repo, we can choose from different sources.
!["Repo Connection"](img/00.PNG)

The prebuilt template for android contains all the required steps to generate a non-signed apk.
!["Task Template"](img/01.PNG)

For generate a signed apk, we must provision the jks file and credentials for signing the build
!["Signing Configuration"](img/02.PNG)

The agent for running the pipeline, it will run in almost every agent, but for best result choose mac or linux distribution
!["Agent Selection"](img/03.PNG)


Last step is save and queue pipeline

!["Save Pipeline"](img/04.PNG)

Build Results
!["Results"](img/05.PNG)



## Continuous Delivery
Currently exist some steps, but for integrating with Official Stores we highly recommend working with AppCenter CD.
