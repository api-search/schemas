---
description: A Knox simple descriptor
layout: schema
name: Descriptor
properties_list:
- description: Descriptor name
  name: name
  type: string
- description: Service discovery type
  name: discoveryType
  type: string
- description: Discovery service address
  name: discoveryAddress
  type: string
- description: Cluster name
  name: cluster
  type: string
- description: Referenced provider configuration
  name: providerConfig
  type: string
- description: Services exposed by this descriptor
  name: services
  type: array
provider_name: Apache Knox
provider_slug: apache-knox
schema_file: json-schema/admin-api-descriptor-schema.json
slug: admin-api-descriptor
tags:
- API Gateway
- Authentication
- Hadoop
- Open Source
- Security
- SSO
title: Descriptor
---
