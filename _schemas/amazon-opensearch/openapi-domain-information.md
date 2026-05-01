---
description: DomainInformation schema from Amazon OpenSearch Service API
layout: schema
name: DomainInformation
properties_list:
- description: ''
  name: OwnerId
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: Region
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-domain-information-schema.json
slug: openapi-domain-information
source_filename: openapi-domain-information-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-information-schema.json\",\n  \"title\": \"DomainInformation\",\n  \"description\": \"DomainInformation schema from Amazon OpenSearch Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OwnerId\": {\n      \"$ref\": \"#/components/schemas/OwnerId\"\n    },\n    \"DomainName\": {\n      \"$ref\": \"#/components/schemas/DomainName\"\n    },\n    \"Region\": {\n      \"$ref\": \"#/components/schemas/Region\"\n    }\n  },\n  \"required\": [\n    \"DomainName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-information-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DomainInformation
---
