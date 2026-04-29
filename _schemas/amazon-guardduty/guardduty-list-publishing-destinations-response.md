---
description: ListPublishingDestinationsResponse schema from Amazon GuardDuty API
layout: schema
name: ListPublishingDestinationsResponse
properties_list:
- description: ''
  name: Destinations
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-list-publishing-destinations-response-schema.json
slug: guardduty-list-publishing-destinations-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-publishing-destinations-response-schema.json\",\n  \"title\": \"ListPublishingDestinationsResponse\",\n  \"description\": \"ListPublishingDestinationsResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Destinations\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinations\"\n          },\n          \"description\": \"A <code>Destinations</code> object that includes information about each publishing destination returned.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"\
  nextToken\"\n          },\n          \"description\": \"A token to use for paginating results that are returned in the response. Set the value of this parameter to null for the first request to a list action. For subsequent calls, use the <code>NextToken</code> value returned from the previous request to continue listing results after the first page.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Destinations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-list-publishing-destinations-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: ListPublishingDestinationsResponse
---
