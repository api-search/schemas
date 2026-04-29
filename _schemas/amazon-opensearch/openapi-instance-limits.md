---
description: InstanceLimits represents the list of instance related attributes that are available for given InstanceType.
layout: schema
name: InstanceLimits
properties_list:
- description: ''
  name: InstanceCountLimits
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-instance-limits-schema.json
slug: openapi-instance-limits
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-instance-limits-schema.json\",\n  \"title\": \"InstanceLimits\",\n  \"description\": \"InstanceLimits represents the list of instance related attributes that are available for given InstanceType. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceCountLimits\": {\n      \"$ref\": \"#/components/schemas/InstanceCountLimits\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-instance-limits-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: InstanceLimits
---
