---
description: Release schema from Apollo Config Open API
layout: schema
name: Release
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: appId
  type: string
- description: ''
  name: clusterName
  type: string
- description: ''
  name: namespaceName
  type: string
- description: Release title
  name: name
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: isAbandoned
  type: boolean
- description: Key-value configuration snapshot at release time
  name: configurations
  type: object
- description: ''
  name: dataChangeCreatedBy
  type: string
- description: ''
  name: dataChangeLastModifiedBy
  type: string
- description: ''
  name: dataChangeCreatedTime
  type: string
- description: ''
  name: dataChangeLastModifiedTime
  type: string
provider_name: Apollo Config
provider_slug: apollo-config
schema_file: json-schema/apollo-open-api-release-schema.json
slug: apollo-open-api-release
tags:
- Apache 2.0
- Configuration Management
- Ctrip
- Distributed Systems
- Java
- Microservices
- Open Source
- Real-Time Configuration
title: Release
---
