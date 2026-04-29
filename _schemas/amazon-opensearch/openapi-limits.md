---
description: Limits for given InstanceType and for each of it's role. <br/> Limits contains following <code> <a>StorageTypes,</a> </code> <code> <a>InstanceLimits</a> </code> and <code> <a>AdditionalLimits</a> </code>
layout: schema
name: Limits
properties_list:
- description: ''
  name: StorageTypes
  type: object
- description: ''
  name: InstanceLimits
  type: object
- description: ''
  name: AdditionalLimits
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-limits-schema.json
slug: openapi-limits
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-limits-schema.json\",\n  \"title\": \"Limits\",\n  \"description\": \" Limits for given InstanceType and for each of it's role. <br/> Limits contains following <code> <a>StorageTypes,</a> </code> <code> <a>InstanceLimits</a> </code> and <code> <a>AdditionalLimits</a> </code> \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StorageTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageTypeList\"\n        },\n        {\n          \"description\": \"StorageType represents the list of storage related types and attributes that are available for given InstanceType. \"\n        }\n      ]\n    },\n    \"InstanceLimits\": {\n      \"$ref\": \"#/components/schemas/InstanceLimits\"\n    },\n    \"AdditionalLimits\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/AdditionalLimitList\"\n        },\n        {\n          \"description\": \" List of additional limits that are specific to a given InstanceType and for each of it's <code> <a>InstanceRole</a> </code> . \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-limits-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: Limits
---
