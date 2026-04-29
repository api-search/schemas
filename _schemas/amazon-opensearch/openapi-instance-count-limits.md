---
description: InstanceCountLimits represents the limits on number of instances that be created in Amazon Elasticsearch for given InstanceType.
layout: schema
name: InstanceCountLimits
properties_list:
- description: ''
  name: MinimumInstanceCount
  type: object
- description: ''
  name: MaximumInstanceCount
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-instance-count-limits-schema.json
slug: openapi-instance-count-limits
source_filename: openapi-instance-count-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-instance-count-limits-schema.json\",\n  \"title\": \"InstanceCountLimits\",\n  \"description\": \" InstanceCountLimits represents the limits on number of instances that be created in Amazon Elasticsearch for given InstanceType. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MinimumInstanceCount\": {\n      \"$ref\": \"#/components/schemas/MinimumInstanceCount\"\n    },\n    \"MaximumInstanceCount\": {\n      \"$ref\": \"#/components/schemas/MaximumInstanceCount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-instance-count-limits-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: InstanceCountLimits
---
