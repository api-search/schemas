---
description: Information about an alarm.
layout: schema
name: Alarm
properties_list:
- description: ''
  name: name
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-alarm-schema.json
slug: amazon-codedeploy-alarm
source_filename: amazon-codedeploy-alarm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-alarm-schema.json\",\n  \"title\": \"Alarm\",\n  \"description\": \"Information about an alarm.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmName\"\n        },\n        {\n          \"description\": \"The name of the alarm. Maximum length is 255 characters. Each alarm name can be used only once in a list of alarms.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-alarm-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: Alarm
---
