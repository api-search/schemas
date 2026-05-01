---
description: DescribeScheduledAuditResponse schema
layout: schema
name: DescribeScheduledAuditResponse
properties_list:
- description: ''
  name: frequency
  type: object
- description: ''
  name: dayOfMonth
  type: object
- description: ''
  name: dayOfWeek
  type: object
- description: ''
  name: targetCheckNames
  type: object
- description: ''
  name: scheduledAuditName
  type: object
- description: ''
  name: scheduledAuditArn
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-scheduled-audit-response-schema.json
slug: iot-core-describe-scheduled-audit-response
source_filename: iot-core-describe-scheduled-audit-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-scheduled-audit-response-schema.json\",\n  \"title\": \"DescribeScheduledAuditResponse\",\n  \"description\": \"DescribeScheduledAuditResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"frequency\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditFrequency\"\n        },\n        {\n          \"description\": \"How often the scheduled audit takes place, either one of <code>DAILY</code>, <code>WEEKLY</code>, <code>BIWEEKLY</code>, or <code>MONTHLY</code>. The start time of each audit is determined by the system.\"\n        }\n      ]\n    },\n    \"dayOfMonth\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfMonth\"\n        },\n        {\n          \"description\": \"The day of the month on which the\
  \ scheduled audit takes place. This is will be <code>1</code> through <code>31</code> or <code>LAST</code>. If days <code>29</code>-<code>31</code> are specified, and the month does not have that many days, the audit takes place on the <code>LAST</code> day of the month.\"\n        }\n      ]\n    },\n    \"dayOfWeek\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DayOfWeek\"\n        },\n        {\n          \"description\": \"The day of the week on which the scheduled audit takes place, either one of <code>SUN</code>, <code>MON</code>, <code>TUE</code>, <code>WED</code>, <code>THU</code>, <code>FRI</code>, or <code>SAT</code>.\"\n        }\n      ]\n    },\n    \"targetCheckNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetAuditCheckNames\"\n        },\n        {\n          \"description\": \"Which checks are performed during the scheduled audit. Checks must be enabled for your account. (Use <code>DescribeAccountAuditConfiguration</code>\
  \ to see the list of all checks, including those that are enabled or use <code>UpdateAccountAuditConfiguration</code> to select which checks are enabled.)\"\n        }\n      ]\n    },\n    \"scheduledAuditName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAuditName\"\n        },\n        {\n          \"description\": \"The name of the scheduled audit.\"\n        }\n      ]\n    },\n    \"scheduledAuditArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScheduledAuditArn\"\n        },\n        {\n          \"description\": \"The ARN of the scheduled audit.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-scheduled-audit-response-schema.json
tags:
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeScheduledAuditResponse
---
