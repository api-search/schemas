---
description: AlarmModelVersionSummaries schema
layout: schema
name: AlarmModelVersionSummaries
properties_list: []
provider_name: Amazon IoT Events
provider_slug: amazon-iot-events
schema_file: json-schema/iot-events-alarm-model-version-summaries-schema.json
slug: iot-events-alarm-model-version-summaries
source_filename: iot-events-alarm-model-version-summaries-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-model-version-summaries-schema.json\",\n  \"title\": \"AlarmModelVersionSummaries\",\n  \"description\": \"AlarmModelVersionSummaries schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"alarmModelName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AlarmModelName\"\n          },\n          {\n            \"description\": \"The name of the alarm model.\"\n          }\n        ]\n      },\n      \"alarmModelArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AlarmModelArn\"\n          },\n          {\n            \"description\": \"The ARN of the alarm model. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\
  \">Amazon Resource Names (ARNs)</a> in the <i>AWS General Reference</i>.\"\n          }\n        ]\n      },\n      \"alarmModelVersion\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AlarmModelVersion\"\n          },\n          {\n            \"description\": \"The version of the alarm model.\"\n          }\n        ]\n      },\n      \"roleArn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AmazonResourceName\"\n          },\n          {\n            \"description\": \"The ARN of the IAM role that allows the alarm to perform actions and access AWS resources. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>AWS General Reference</i>.\"\n          }\n        ]\n      },\n      \"creationTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n\
  \          {\n            \"description\": \"The time the alarm model was created, in the Unix epoch format.\"\n          }\n        ]\n      },\n      \"lastUpdateTime\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/Timestamp\"\n          },\n          {\n            \"description\": \"The time the alarm model was last updated, in the Unix epoch format.\"\n          }\n        ]\n      },\n      \"status\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AlarmModelVersionStatus\"\n          },\n          {\n            \"description\": \"<p>The status of the alarm model. The status can be one of the following values:</p> <ul> <li> <p> <code>ACTIVE</code> - The alarm model is active and it's ready to evaluate data.</p> </li> <li> <p> <code>ACTIVATING</code> - AWS IoT Events is activating your alarm model. Activating an alarm model can take up to a few minutes.</p> </li> <li> <p> <code>INACTIVE</code> - The alarm model\
  \ is inactive, so it isn't ready to evaluate data. Check your alarm model information and update the alarm model.</p> </li> <li> <p> <code>FAILED</code> - You couldn't create or update the alarm model. Check your alarm model information and try again.</p> </li> </ul>\"\n          }\n        ]\n      },\n      \"statusMessage\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/StatusMessage\"\n          },\n          {\n            \"description\": \" Contains information about the status of the alarm model version. \"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains a summary of an alarm model version.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-events/refs/heads/main/json-schema/iot-events-alarm-model-version-summaries-schema.json
tags:
- Event Detection
- IoT
- State Machine
- Automation
title: AlarmModelVersionSummaries
---
