---
description: A subset of the attributes that describe a log group. In CloudWatch a log group is a group of log streams that share the same retention, monitoring, and access control settings.
layout: schema
name: LogGroupSummary
properties_list:
- description: ''
  name: logGroupName
  type: object
- description: ''
  name: logType
  type: object
provider_name: Amazon Mainframe Modernization
provider_slug: amazon-mainframe-modernization
schema_file: json-schema/amazon-mainframe-modernization-log-group-summary-schema.json
slug: amazon-mainframe-modernization-log-group-summary
source_filename: amazon-mainframe-modernization-log-group-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-log-group-summary-schema.json\",\n  \"title\": \"LogGroupSummary\",\n  \"description\": \"A subset of the attributes that describe a log group. In CloudWatch a log group is a group of log streams that share the same retention, monitoring, and access control settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupIdentifier\"\n        },\n        {\n          \"description\": \"The name of the log group.\"\n        }\n      ]\n    },\n    \"logType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String20\"\n        },\n        {\n          \"description\": \"The type of log.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"logGroupName\",\n    \"logType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mainframe-modernization/refs/heads/main/json-schema/amazon-mainframe-modernization-log-group-summary-schema.json
tags:
- AWS
- COBOL
- Mainframe
- Migration
- Modernization
- Batch Processing
title: LogGroupSummary
---
