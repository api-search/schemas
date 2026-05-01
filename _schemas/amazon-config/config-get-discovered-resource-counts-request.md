---
description: GetDiscoveredResourceCountsRequest schema
layout: schema
name: GetDiscoveredResourceCountsRequest
properties_list:
- description: ''
  name: resourceTypes
  type: object
- description: ''
  name: limit
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-get-discovered-resource-counts-request-schema.json
slug: config-get-discovered-resource-counts-request
source_filename: config-get-discovered-resource-counts-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-discovered-resource-counts-request-schema.json\",\n  \"title\": \"GetDiscoveredResourceCountsRequest\",\n  \"description\": \"GetDiscoveredResourceCountsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceTypes\"\n        },\n        {\n          \"description\": \"<p>The comma-separated list that specifies the resource types that you want Config to return (for example, <code>\\\"AWS::EC2::Instance\\\"</code>, <code>\\\"AWS::IAM::User\\\"</code>).</p> <p>If a value for <code>resourceTypes</code> is not specified, Config returns all resource types that Config is recording in the region for your account.</p> <note> <p>If the configuration recorder is turned off, Config returns\
  \ an empty list of <a>ResourceCount</a> objects. If the configuration recorder is not recording a specific resource type (for example, S3 buckets), that resource type is not returned in the list of <a>ResourceCount</a> objects.</p> </note>\"\n        }\n      ]\n    },\n    \"limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of <a>ResourceCount</a> objects returned on each page. The default is 100. You cannot specify a number greater than 100. If you specify 0, Config uses the default.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"The <code>nextToken</code> string returned on a previous page that you use to get the next page of results in a paginated response.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-get-discovered-resource-counts-request-schema.json
tags:
- Auditing
- Compliance
- Configuration Management
- Governance
- Security
title: GetDiscoveredResourceCountsRequest
---
