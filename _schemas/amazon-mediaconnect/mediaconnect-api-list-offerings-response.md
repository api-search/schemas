---
description: ListOfferingsResponse schema from AWS Elemental MediaConnect API
layout: schema
name: ListOfferingsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Offerings
  type: object
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
schema_file: json-schema/mediaconnect-api-list-offerings-response-schema.json
slug: mediaconnect-api-list-offerings-response
source_filename: mediaconnect-api-list-offerings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-list-offerings-response-schema.json\",\n  \"title\": \"ListOfferingsResponse\",\n  \"description\": \"ListOfferingsResponse schema from AWS Elemental MediaConnect API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"The token that identifies which batch of results that you want to see. For example, you submit a ListOfferings request with MaxResults set at 5. The service returns the first batch of results (up to 5) and a NextToken value. To see the next batch of results, you can submit the ListOfferings request a second time and specify the NextToken value.\"\
  \n        }\n      ]\n    },\n    \"Offerings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOffering\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offerings\"\n          },\n          \"description\": \"A list of offerings that are available to this account in the current AWS Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconnect/refs/heads/main/json-schema/mediaconnect-api-list-offerings-response-schema.json
tags:
- AWS
- Broadcasting
- Live Video
- Media
- Media Transport
title: ListOfferingsResponse
---
