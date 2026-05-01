---
description: Contains information about the publishing destination, including the ID, type, and status.
layout: schema
name: Destination
properties_list:
- description: ''
  name: DestinationId
  type: object
- description: ''
  name: DestinationType
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-destination-schema.json
slug: guardduty-destination
source_filename: guardduty-destination-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-destination-schema.json\",\n  \"title\": \"Destination\",\n  \"description\": \"Contains information about the publishing destination, including the ID, type, and status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationId\"\n          },\n          \"description\": \"The unique ID of the publishing destination.\"\n        }\n      ]\n    },\n    \"DestinationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationType\"\n          },\n          \"description\": \"The type of resource\
  \ used for the publishing destination. Currently, only Amazon S3 buckets are supported.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublishingStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The status of the publishing destination.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DestinationId\",\n    \"DestinationType\",\n    \"Status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-destination-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Destination
---
