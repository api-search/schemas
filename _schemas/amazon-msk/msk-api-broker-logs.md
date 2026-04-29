---
description: BrokerLogs schema from Amazon MSK API
layout: schema
name: BrokerLogs
properties_list:
- description: ''
  name: CloudWatchLogs
  type: object
- description: ''
  name: Firehose
  type: object
- description: ''
  name: S3
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-broker-logs-schema.json
slug: msk-api-broker-logs
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-logs-schema.json\",\n  \"title\": \"BrokerLogs\",\n  \"description\": \"BrokerLogs schema from Amazon MSK API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudWatchLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudWatchLogs\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"cloudWatchLogs\"\n          }\n        }\n      ]\n    },\n    \"Firehose\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Firehose\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"firehose\"\n          }\n        }\n      ]\n    },\n    \"S3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3\"\
  \n          }\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-broker-logs-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: BrokerLogs
---
