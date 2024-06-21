# rstudio-images

## Workbench image
image:
  dockerImage: rstudio/rstudio-workbench:ubuntu2204-2024.04.2
  dockerFileReference: https://raw.githubusercontent.com/rstudio/rstudio-docker-products/dev/workbench/Dockerfile.ubuntu2204
  description: rstudio workbench
  type: application_tool
  dockerSHA: sha256:a894a8e272f5061094767c99bd83db7f4bdd19c3b1db2d640b0f057b3d25d17f


## R session complete image
image:
  dockerImage: rstudio/r-session-complete:ubuntu2204-2024.04.2
  dockerFileReference: https://raw.githubusercontent.com/rstudio/rstudio-docker-products/dev/r-session-complete/Dockerfile.ubuntu2204
  description: rstudio workbench r-session
  type: application_tool
  dockerSHA: sha256:4b8d11524cd328732a0bf40e6a97b595d124a4951361a43080f5165db1951435


## Connect image
image:
  dockerImage: rstudio/rstudio-connect:ubuntu2204-2024.05.0
  dockerFileReference: https://raw.githubusercontent.com/rstudio/rstudio-docker-products/dev/connect/Dockerfile.ubuntu2204
  description: rstudio connect
  type: application_tool
  dockerSHA: sha256:b3a0691c3a333fe93b29f305d6cb34d6751d683d265d92de0bac3903a60a401e


## Init Container image
image:
  dockerImage: rstudio/rstudio-connect-content-init:ubuntu2204-2024.05.0
  dockerFileReference: https://raw.githubusercontent.com/rstudio/rstudio-docker-products/dev/connect-content-init/Dockerfile.ubuntu2204
  description: rstudio connect init container
  type: application_tool
  dockerSHA: sha256:eb7ccdcf47414c9505db85a87c1e5282658933caa9d0d09ab2f33e540cf3e441


## Content base image
#### 	We don't need this image if we will be using the content pro image. Content pro images include posit professional drivers.
#### 	https://docs.posit.co/pro-drivers/
image:
  dockerImage: rstudio/content-base:r4.3.3-py3.12.3-ubuntu2204
  dockerFileReference: https://raw.githubusercontent.com/rstudio/rstudio-docker-products/dev/content/base/Dockerfile.ubuntu2204
  description: rstudio connect content base image
  type: application_tool
  dockerSHA: sha256:5114613a7cc6c079fe4b26e4799be5db9a73edbb6a337541063995e195a68c5b


## Content pro image
image:
  dockerImage: rstudio/content-pro:r4.3.3-py3.12.3-ubuntu2204
  dockerFileReference: https://raw.githubusercontent.com/rstudio/rstudio-docker-products/dev/content/pro/Dockerfile.ubuntu2204
  description: rstudio connect content pro image
  type: application_tool
  dockerSHA: sha256:201f3f7f3de13210e16c44a7e79e47dd032aeff3b27aa0e3030532772e0aaa9a
