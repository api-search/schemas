---
description: CreatePublishingDestinationResponse schema from Amazon GuardDuty API
layout: schema
name: CreatePublishingDestinationResponse
properties_list:
- description: ''
  name: DestinationId
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-create-publishing-destination-response-schema.json
slug: guardduty-create-publishing-destination-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-publishing-destination-response-schema.json\",\n  \"title\": \"CreatePublishingDestinationResponse\",\n  \"description\": \"CreatePublishingDestinationResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationId\"\n          },\n          \"description\": \"The ID of the publishing destination that is created.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DestinationId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-publishing-destination-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreatePublishingDestinationResponse
---
