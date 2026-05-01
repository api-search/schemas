---
description: ListClustersRequest schema from Amazon Snow Family API
layout: schema
name: ListClustersRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-clusters-request-schema.json
slug: amazon-snow-family-list-clusters-request
source_filename: amazon-snow-family-list-clusters-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-clusters-request-schema.json\",\n  \"title\": \"ListClustersRequest\",\n  \"description\": \"ListClustersRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListLimit\"\n        },\n        {\n          \"description\": \"The number of <code>ClusterListEntry</code> objects to return.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP requests are stateless. To identify what object comes \\\"next\\\" in the list of <code>ClusterListEntry</code> objects, you have the option of specifying <code>NextToken</code>\
  \ as the starting point for your returned list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-clusters-request-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListClustersRequest
---
