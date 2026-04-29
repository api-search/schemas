---
description: CreatePublishingDestinationRequest schema from Amazon GuardDuty API
layout: schema
name: CreatePublishingDestinationRequest
properties_list:
- description: ''
  name: DestinationType
  type: object
- description: ''
  name: DestinationProperties
  type: object
- description: ''
  name: ClientToken
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-create-publishing-destination-request-schema.json
slug: guardduty-create-publishing-destination-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-publishing-destination-request-schema.json\",\n  \"title\": \"CreatePublishingDestinationRequest\",\n  \"description\": \"CreatePublishingDestinationRequest schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationType\"\n          },\n          \"description\": \"The type of resource for the publishing destination. Currently only Amazon S3 buckets are supported.\"\n        }\n      ]\n    },\n    \"DestinationProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationProperties\"\n        },\n        {\n          \"xml\"\
  : {\n            \"name\": \"destinationProperties\"\n          },\n          \"description\": \"The properties of the publishing destination, including the ARNs for the destination and the KMS key used for encryption.\"\n        }\n      ]\n    },\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientToken\"\n          },\n          \"description\": \"The idempotency token for the request.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DestinationType\",\n    \"DestinationProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-create-publishing-destination-request-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: CreatePublishingDestinationRequest
---
