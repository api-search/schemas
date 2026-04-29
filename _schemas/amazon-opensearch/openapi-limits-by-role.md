---
description: 'Map of Role of the Instance and Limits that are applicable. Role performed by given Instance in Elasticsearch can be one of the following: <ul> <li>data: If the given InstanceType is used as data node</li> <li>master: If the given InstanceType is used as master node</li> <li>ultra_warm: If the given InstanceType is used as warm node</li> </ul>'
layout: schema
name: LimitsByRole
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-limits-by-role-schema.json
slug: openapi-limits-by-role
source_filename: openapi-limits-by-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-limits-by-role-schema.json\",\n  \"title\": \"LimitsByRole\",\n  \"description\": \" Map of Role of the Instance and Limits that are applicable. Role performed by given Instance in Elasticsearch can be one of the following: <ul> <li>data: If the given InstanceType is used as data node</li> <li>master: If the given InstanceType is used as master node</li> <li>ultra_warm: If the given InstanceType is used as warm node</li> </ul> \",\n  \"type\": \"object\",\n  \"additionalProperties\": {\n    \"$ref\": \"#/components/schemas/Limits\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-limits-by-role-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: LimitsByRole
---
