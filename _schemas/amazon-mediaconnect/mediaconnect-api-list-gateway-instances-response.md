---
description: ListGatewayInstancesResponse schema from AWS Elemental MediaConnect API
layout: schema
name: ListGatewayInstancesResponse
properties_list:
- description: ''
  name: Instances
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-list-gateway-instances-response-schema.json
slug: mediaconnect-api-list-gateway-instances-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-list-gateway-instances-response-schema.json\",\n  \"title\": \"ListGatewayInstancesResponse\",\n  \"description\": \"ListGatewayInstancesResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Instances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfListedGatewayInstance\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"instances\"\n          },\n          \"description\": \"A list of instance summaries.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The token\
  \ that identifies which batch of results that you want to see. For example, you submit a ListInstances request with MaxResults set at 5. The service returns the first batch of results (up to 5) and a NextToken value. To see the next batch of results, you can submit the ListInstances request a second time and specify the NextToken value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-list-gateway-instances-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: ListGatewayInstancesResponse
---
