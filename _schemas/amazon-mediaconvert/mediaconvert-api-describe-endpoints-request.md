---
description: DescribeEndpointsRequest
layout: schema
name: DescribeEndpointsRequest
properties_list:
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: Mode
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-describe-endpoints-request-schema.json
slug: mediaconvert-api-describe-endpoints-request
source_filename: mediaconvert-api-describe-endpoints-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-describe-endpoints-request-schema.json\",\n  \"title\": \"DescribeEndpointsRequest\",\n  \"description\": \"DescribeEndpointsRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"maxResults\"\n          },\n          \"description\": \"Optional. Max number of endpoints, up to twenty, that will be returned at one time.\"\n        }\n      ]\n    },\n    \"Mode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribeEndpointsMode\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"mode\"\n          },\n          \"description\": \"Optional field, defaults\
  \ to DEFAULT. Specify DEFAULT for this operation to return your endpoints if any exist, or to create an endpoint for you and return it if one doesn't already exist. Specify GET_ONLY to return your endpoints if any exist, or an empty list if none exist.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Use this string, provided with the response to a previous request, to request the next batch of endpoints.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-describe-endpoints-request-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: DescribeEndpointsRequest
---
