---
description: CreateViewRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: CreateViewRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: schema
  type: object
- description: The view version to create, will replace the schema-id sent within the view-version with the id assigned to the provided schema
  name: view-version
  type: object
- description: ''
  name: properties
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-create-view-request-schema.json
slug: rest-catalog-open-api-create-view-request
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CreateViewRequest
---
