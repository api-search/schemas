---
description: Information about alarms associated with a deployment or deployment group.
layout: schema
name: AlarmConfiguration
properties_list:
- description: ''
  name: enabled
  type: object
- description: ''
  name: ignorePollAlarmFailure
  type: object
- description: ''
  name: alarms
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-alarm-configuration-schema.json
slug: amazon-codedeploy-alarm-configuration
source_filename: amazon-codedeploy-alarm-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-alarm-configuration-schema.json\",\n  \"title\": \"AlarmConfiguration\",\n  \"description\": \"Information about alarms associated with a deployment or deployment group.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Indicates whether the alarm configuration is enabled.\"\n        }\n      ]\n    },\n    \"ignorePollAlarmFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Indicates whether a deployment should continue if information about the current state of alarms cannot be retrieved from Amazon CloudWatch. The default value\
  \ is false.</p> <ul> <li> <p> <code>true</code>: The deployment proceeds even if alarm status information can't be retrieved from Amazon CloudWatch.</p> </li> <li> <p> <code>false</code>: The deployment stops if alarm status information can't be retrieved from Amazon CloudWatch.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"alarms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlarmList\"\n        },\n        {\n          \"description\": \"A list of alarms configured for the deployment or deployment group. A maximum of 10 alarms can be added.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-alarm-configuration-schema.json
tags:
- Amazon
- AWS
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: AlarmConfiguration
---
