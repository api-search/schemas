---
description: DescribePublishingDestinationResponse schema from Amazon GuardDuty API
layout: schema
name: DescribePublishingDestinationResponse
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
- description: ''
  name: PublishingFailureStartTimestamp
  type: object
- description: ''
  name: DestinationProperties
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-describe-publishing-destination-response-schema.json
slug: guardduty-describe-publishing-destination-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-describe-publishing-destination-response-schema.json\",\n  \"title\": \"DescribePublishingDestinationResponse\",\n  \"description\": \"DescribePublishingDestinationResponse schema from Amazon GuardDuty API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DestinationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationId\"\n          },\n          \"description\": \"The ID of the publishing destination.\"\n        }\n      ]\n    },\n    \"DestinationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"destinationType\"\n          },\n          \"description\"\
  : \"The type of publishing destination. Currently, only Amazon S3 buckets are supported.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublishingStatus\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The status of the publishing destination.\"\n        }\n      ]\n    },\n    \"PublishingFailureStartTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"publishingFailureStartTimestamp\"\n          },\n          \"description\": \"The time, in epoch millisecond format, at which GuardDuty was first unable to publish findings to the destination.\"\n        }\n      ]\n    },\n    \"DestinationProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationProperties\"\n        },\n       \
  \ {\n          \"xml\": {\n            \"name\": \"destinationProperties\"\n          },\n          \"description\": \"A <code>DestinationProperties</code> object that includes the <code>DestinationArn</code> and <code>KmsKeyArn</code> of the publishing destination.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DestinationId\",\n    \"DestinationType\",\n    \"Status\",\n    \"PublishingFailureStartTimestamp\",\n    \"DestinationProperties\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-describe-publishing-destination-response-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: DescribePublishingDestinationResponse
---
