---
description: repositoryParameterAnnouncement schema from Argo CD API
layout: schema
name: repositoryParameterAnnouncement
properties_list:
- description: array is the default value of the parameter if the parameter is an array.
  name: array
  type: array
- description: collectionType is the type of value this parameter holds - either a single value (a string) or a collection (array or map). If collectionType is set, only the field with that type will be used. If col
  name: collectionType
  type: string
- description: itemType determines the primitive data type represented by the parameter. Parameters are always encoded as strings, but this field lets them be interpreted as other primitive types.
  name: itemType
  type: string
- description: map is the default value of the parameter if the parameter is a map.
  name: map
  type: object
- description: name is the name identifying a parameter.
  name: name
  type: string
- description: required defines if this given parameter is mandatory.
  name: required
  type: boolean
- description: string is the default value of the parameter if the parameter is a string.
  name: string
  type: string
- description: title is a human-readable text of the parameter name.
  name: title
  type: string
- description: tooltip is a human-readable description of the parameter.
  name: tooltip
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-repository-parameter-announcement-schema.json
slug: argo-cd-repository-parameter-announcement
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: repositoryParameterAnnouncement
---
