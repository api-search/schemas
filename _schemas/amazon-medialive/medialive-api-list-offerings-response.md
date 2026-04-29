---
description: Placeholder documentation for ListOfferingsResponse
layout: schema
name: ListOfferingsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Offerings
  type: object
provider_name: Amazon MediaLive
provider_slug: amazon-medialive
schema_file: json-schema/medialive-api-list-offerings-response-schema.json
slug: medialive-api-list-offerings-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-offerings-response-schema.json\",\n  \"title\": \"ListOfferingsResponse\",\n  \"description\": \"Placeholder documentation for ListOfferingsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"nextToken\"\n          },\n          \"description\": \"Token to retrieve the next page of results\"\n        }\n      ]\n    },\n    \"Offerings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfOffering\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"offerings\"\n          },\n          \"description\": \"List of offerings\"\n        }\n      ]\n    }\n\
  \  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-medialive/refs/heads/main/json-schema/medialive-api-list-offerings-response-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ListOfferingsResponse
---
