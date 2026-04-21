---
description: A workspace resource.
layout: schema
name: Workspace
properties_list:
- description: Resource ID
  name: id
  type: string
- description: Resource name
  name: name
  type: string
- description: Resource type
  name: type
  type: string
- description: Azure region location
  name: location
  type: string
- description: Resource tags
  name: tags
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: azure-synapse
schema_file: json-schema/azure-synapse-workspace-schema.json
slug: azure-synapse-workspace
tags:
- Analytics
- Apache Spark
- Big Data
- Data Warehouse
- ETL
- SQL
title: Workspace
---
