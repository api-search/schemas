---
description: CommitTableRequest schema from Apache Iceberg REST Catalog API
layout: schema
name: CommitTableRequest
properties_list:
- description: Table identifier to update; must be present for CommitTransactionRequest
  name: identifier
  type: object
- description: ''
  name: requirements
  type: array
- description: ''
  name: updates
  type: array
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-commit-table-request-schema.json
slug: rest-catalog-open-api-commit-table-request
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: CommitTableRequest
---
