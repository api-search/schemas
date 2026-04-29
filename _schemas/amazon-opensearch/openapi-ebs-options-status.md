---
description: Status of the EBS options for the specified Elasticsearch domain.
layout: schema
name: EBSOptionsStatus
properties_list:
- description: ''
  name: Options
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-ebs-options-status-schema.json
slug: openapi-ebs-options-status
source_filename: openapi-ebs-options-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-ebs-options-status-schema.json\",\n  \"title\": \"EBSOptionsStatus\",\n  \"description\": \" Status of the EBS options for the specified Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Options\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSOptions\"\n        },\n        {\n          \"description\": \" Specifies the EBS options for the specified Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionStatus\"\n        },\n        {\n          \"description\": \" Specifies the status of the EBS options for the specified Elasticsearch domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Options\",\n    \"Status\"\n  ]\n\
  }"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-ebs-options-status-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: EBSOptionsStatus
---
