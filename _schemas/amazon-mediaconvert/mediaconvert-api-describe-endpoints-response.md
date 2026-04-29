---
description: DescribeEndpointsResponse schema from Amazon MediaConvert API
layout: schema
name: DescribeEndpointsResponse
properties_list:
- description: ''
  name: Endpoints
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-describe-endpoints-response-schema.json
slug: mediaconvert-api-describe-endpoints-response
source_filename: mediaconvert-api-describe-endpoints-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-describe-endpoints-response-schema.json\",\n  \"title\": \"DescribeEndpointsResponse\",\n  \"description\": \"DescribeEndpointsResponse schema from Amazon MediaConvert API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Endpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfEndpoint\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endpoints\"\n          },\n          \"description\": \"List of endpoints\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Use this string to request the next batch of endpoints.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-describe-endpoints-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: DescribeEndpointsResponse
---
