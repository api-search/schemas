---
description: An Apptainer container image (SIF file) for HPC and scientific computing
layout: schema
name: ContainerImage
properties_list:
- description: Unique container image identifier
  name: imageId
  type: string
- description: Container image name
  name: name
  type: string
- description: Container image version
  name: version
  type: string
- description: Source URI (docker://image, library://image, oras://, etc.)
  name: source
  type: string
- description: Container image format
  name: format
  type: string
- description: Image size in bytes
  name: size
  type: integer
- description: Image creation timestamp
  name: createdAt
  type: string
- description: SHA-256 hash of the image for verification
  name: sha256
  type: string
provider_name: Apptainer
provider_slug: apptainer
schema_file: json-schema/container-image-schema.json
slug: container-image
tags:
- Containers
- HPC
- Scientific Computing
- Open Source
- Linux Foundation
title: ContainerImage
---
