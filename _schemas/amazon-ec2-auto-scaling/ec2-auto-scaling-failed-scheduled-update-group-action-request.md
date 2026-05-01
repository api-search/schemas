---
description: Describes a scheduled action that could not be created, updated, or deleted.
layout: schema
name: FailedScheduledUpdateGroupActionRequest
properties_list:
- description: ''
  name: ScheduledActionName
  type: object
- description: ''
  name: ErrorCode
  type: object
- description: ''
  name: ErrorMessage
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-failed-scheduled-update-group-action-request-schema.json
slug: ec2-auto-scaling-failed-scheduled-update-group-action-request
source_filename: ec2-auto-scaling-failed-scheduled-update-group-action-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-failed-scheduled-update-group-action-request-schema.json\",\n  \"title\": \"FailedScheduledUpdateGroupActionRequest\",\n  \"description\": \"Describes a scheduled action that could not be created, updated, or deleted.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScheduledActionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the scheduled action.\"\n        }\n      ]\n    },\n    \"ErrorCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen64\"\n        },\n        {\n          \"description\": \"The error code.\"\n        }\n      ]\n    },\n    \"ErrorMessage\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/XmlString\"\n        },\n        {\n          \"description\": \"The error message accompanying the error code.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScheduledActionName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-failed-scheduled-update-group-action-request-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: FailedScheduledUpdateGroupActionRequest
---
