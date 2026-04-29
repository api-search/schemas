---
description: DomainInfo schema from Amazon OpenSearch Service API
layout: schema
name: DomainInfo
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: EngineType
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-domain-info-schema.json
slug: openapi-domain-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-info-schema.json\",\n  \"title\": \"DomainInfo\",\n  \"description\": \"DomainInfo schema from Amazon OpenSearch Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \" Specifies the <code>DomainName</code>.\"\n        }\n      ]\n    },\n    \"EngineType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EngineType\"\n        },\n        {\n          \"description\": \" Specifies the <code>EngineType</code> of the domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-info-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DomainInfo
---
