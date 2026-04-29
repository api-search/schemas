---
description: GetDiscoveredResourceCountsResponse schema
layout: schema
name: GetDiscoveredResourceCountsResponse
properties_list:
- description: ''
  name: totalDiscoveredResources
  type: object
- description: ''
  name: resourceCounts
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-discovered-resource-counts-response-schema.json
slug: config-get-discovered-resource-counts-response
source_filename: config-get-discovered-resource-counts-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-discovered-resource-counts-response-schema.json\",\n  \"title\": \"GetDiscoveredResourceCountsResponse\",\n  \"description\": \"GetDiscoveredResourceCountsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"totalDiscoveredResources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"<p>The total number of resources that Config is recording in the region for your account. If you specify resource types in the request, Config returns only the total number of resources for those resource types.</p> <p class=\\\"title\\\"> <b>Example</b> </p> <ol> <li> <p>Config is recording three resource types in the US East (Ohio) Region for your account: 25 EC2 instances, 20 IAM users, and 15 S3 buckets,\
  \ for a total of 60 resources.</p> </li> <li> <p>You make a call to the <code>GetDiscoveredResourceCounts</code> action and specify the resource type, <code>\\\"AWS::EC2::Instances\\\"</code>, in the request.</p> </li> <li> <p>Config returns 25 for <code>totalDiscoveredResources</code>.</p> </li> </ol>\"\n        }\n      ]\n    },\n    \"resourceCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceCounts\"\n        },\n        {\n          \"description\": \"The list of <code>ResourceCount</code> objects. Each object is listed in descending order by the number of resources.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The string that you use in a subsequent request to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-discovered-resource-counts-response-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: GetDiscoveredResourceCountsResponse
---
