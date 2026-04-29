---
description: Limits that are applicable for given storage type.
layout: schema
name: StorageTypeLimit
properties_list:
- description: ''
  name: LimitName
  type: object
- description: ''
  name: LimitValues
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-storage-type-limit-schema.json
slug: openapi-storage-type-limit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-storage-type-limit-schema.json\",\n  \"title\": \"StorageTypeLimit\",\n  \"description\": \"Limits that are applicable for given storage type. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LimitName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitName\"\n        },\n        {\n          \"description\": \" Name of storage limits that are applicable for given storage type. If <code> <a>StorageType</a> </code> is ebs, following storage options are applicable <ol> <li>MinimumVolumeSize</li> Minimum amount of volume size that is applicable for given storage type.It can be empty if it is not applicable. <li>MaximumVolumeSize</li> Maximum amount of volume size that is applicable for given storage type.It can be empty if it is not applicable. <li>MaximumIops</li>\
  \ Maximum amount of Iops that is applicable for given storage type.It can be empty if it is not applicable. <li>MinimumIops</li> Minimum amount of Iops that is applicable for given storage type.It can be empty if it is not applicable. <li>MaximumThroughput</li> Maximum amount of Throughput that is applicable for given storage type.It can be empty if it is not applicable. <li>MinimumThroughput</li> Minimum amount of Throughput that is applicable for given storage type.It can be empty if it is not applicable. </ol> \"\n        }\n      ]\n    },\n    \"LimitValues\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitValueList\"\n        },\n        {\n          \"description\": \" Values for the <code> <a>StorageTypeLimit$LimitName</a> </code> . \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-storage-type-limit-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: StorageTypeLimit
---
