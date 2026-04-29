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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-load-view-result-schema.json\",\n  \"title\": \"LoadViewResult\",\n  \"description\": \"Result used when a view is successfully loaded.\\n\\n\\nThe view metadata JSON is returned in the `metadata` field. The corresponding file location of view metadata is returned in the `metadata-location` field.\\nClients can check whether metadata has changed by comparing metadata locations after the view has been created.\\n\\nThe `config` map returns view-specific configuration for the view's resources.\\n\\nThe following configurations should be respected by clients:\\n\\n## General Configurations\\n\\n- `token`: Authorization bearer token to use for view requests if OAuth2 security is enabled\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata-location\": {\n      \"type\": \"\
  string\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/ViewMetadata\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"metadata-location\",\n    \"metadata\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-load-view-result-schema.json
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
