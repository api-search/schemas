---
description: Represents a subscriber for Amazon Security Lake data.
layout: schema
name: Subscriber
properties_list:
- description: The unique identifier for the subscriber.
  name: subscriberId
  type: string
- description: The ARN of the subscriber.
  name: subscriberArn
  type: string
- description: The name of the subscriber.
  name: subscriberName
  type: string
- description: A description of the subscriber.
  name: subscriberDescription
  type: string
- description: The status of the subscriber.
  name: subscriberStatus
  type: string
- description: The access types granted to the subscriber.
  name: accessTypes
  type: array
- description: The ARN of the resource share for AWS RAM-based access.
  name: resourceShareArn
  type: string
- description: Timestamp when the subscriber was created.
  name: createdAt
  type: string
- description: Timestamp when the subscriber was last updated.
  name: updatedAt
  type: string
provider_name: Amazon Security Lake
provider_slug: amazon-security-lake
schema_file: json-schema/amazon-security-lake-subscriber-schema.json
slug: amazon-security-lake-subscriber
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/json-schema/amazon-security-lake-subscriber-schema.json\",\n  \"title\": \"Subscriber\",\n  \"description\": \"Represents a subscriber for Amazon Security Lake data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"subscriberId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the subscriber.\",\n      \"example\": \"sub-a1b2c3d4\"\n    },\n    \"subscriberArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the subscriber.\",\n      \"example\": \"arn:aws:securitylake:us-east-1:123456789012:subscriber/sub-a1b2c3d4\"\n    },\n    \"subscriberName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the subscriber.\",\n      \"example\": \"MySIEMSubscriber\"\n    },\n    \"subscriberDescription\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"A description of the subscriber.\"\n    },\n    \"subscriberStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the subscriber.\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"DEACTIVATED\",\n        \"PENDING\",\n        \"READY\"\n      ],\n      \"example\": \"ACTIVE\"\n    },\n    \"accessTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The access types granted to the subscriber.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"LAKEFORMATION\",\n          \"S3\"\n        ]\n      }\n    },\n    \"resourceShareArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the resource share for AWS RAM-based access.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the subscriber was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Timestamp when the subscriber was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-security-lake/refs/heads/main/json-schema/amazon-security-lake-subscriber-schema.json
tags:
- AWS
- Data Lake
- Security
- SIEM
- Threat Detection
title: Subscriber
---
