---
description: ListClusterJobsRequest schema from Amazon Snow Family API
layout: schema
name: ListClusterJobsRequest
properties_list:
- description: ''
  name: ClusterId
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-list-cluster-jobs-request-schema.json
slug: amazon-snow-family-list-cluster-jobs-request
source_filename: amazon-snow-family-list-cluster-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-cluster-jobs-request-schema.json\",\n  \"title\": \"ListClusterJobsRequest\",\n  \"description\": \"ListClusterJobsRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterId\"\n        },\n        {\n          \"description\": \"The 39-character ID for the cluster that you want to list, for example <code>CID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ListLimit\"\n        },\n        {\n          \"description\": \"The number of <code>JobListEntry</code> objects to return.\"\n        }\n      ]\n    },\n    \"NextToken\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"HTTP requests are stateless. To identify what object comes \\\"next\\\" in the list of <code>JobListEntry</code> objects, you have the option of specifying <code>NextToken</code> as the starting point for your returned list.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ClusterId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-list-cluster-jobs-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ListClusterJobsRequest
---
