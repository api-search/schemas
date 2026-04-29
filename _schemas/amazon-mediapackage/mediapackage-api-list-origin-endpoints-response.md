---
description: ListOriginEndpointsResponse schema from Amazon MediaPackage API
layout: schema
name: ListOriginEndpointsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: OriginEndpoints
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-list-origin-endpoints-response-schema.json
slug: mediapackage-api-list-origin-endpoints-response
source_filename: mediapackage-api-list-origin-endpoints-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-list-origin-endpoints-response-schema.json\",\n  \"title\": \"ListOriginEndpointsResponse\",\n  \"description\": \"ListOriginEndpointsResponse schema from Amazon MediaPackage API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"A token that can be used to resume pagination from the end of the collection.\"\n        }\n      ]\n    },\n    \"OriginEndpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOriginEndpoint\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"originEndpoints\"\n    \
  \      },\n          \"description\": \"A list of OriginEndpoint records.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-list-origin-endpoints-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListOriginEndpointsResponse
---
