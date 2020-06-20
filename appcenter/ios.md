# Welcome
This file contains examples to create CI/CD experiences for iOS target.

The first task is upload our ios repository if we want to keep track inside Azure DevOps, but we can use other sources instead.

## Continuous Integration
When we create a new project, is required to specify what is going to be the target OS and the base technology, we can change it later.
!["Project Setup"](img/00.png "Project Setup")
!["Project Configuration"](img/i_01.png "Project Configuration")


The first thing is connecting the repo, we can choose from different sources.
!["Repo Connection"](img/i_02.png "Repo Connection")

Once the connection is completed, we can choose from the different branches to configure a build pipeline.
!["Branch Selection"](img/i_03.png "Branch Selection")
!["Build Configuration"](img/i_04.png "Build Configuration")

For generate a signed apk, we must provision the p12 and mobileprovisioning file for signing the build
!["Signing Configuration"](img/i_05.png "Signing Configuration")


Last step is save and queue pipeline and check results
!["Save Pipeline"](img/i_06.png "Save Pipeline")

## Continuous Delivery
For accomplish this task, we can distribute using AppCenter mechanism or Test Flight for sending to a group or groups and connect to store
!["Results"](img/a_07.png "Results")