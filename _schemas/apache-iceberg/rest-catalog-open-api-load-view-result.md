---
description: 'Result used when a view is successfully loaded. The view metadata JSON is returned in the `metadata` field. The corresponding file location of view metadata is returned in the `metadata-location` field. Clients can check whether metadata has changed by comparing metadata locations after the view has been created. The `config` map returns view-specific configuration for the view''s resources. The following configurations should be respected by clients: ## General Configurations - `token`: Authorization bearer token to use for view requests if OAuth2 security is enabled'
layout: schema
name: LoadViewResult
properties_list:
- description: ''
  name: metadata-location
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: config
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-load-view-result-schema.json
slug: rest-catalog-open-api-load-view-result
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: LoadViewResult
---
