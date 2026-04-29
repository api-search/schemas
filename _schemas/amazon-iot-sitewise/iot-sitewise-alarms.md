---
description: Contains the configuration information of an alarm created in an IoT SiteWise Monitor portal. You can use the alarm to monitor an asset property and get notified when the asset property value is outside a specified range. For more information, see <a href="https://docs.aws.amazon.com/iot-sitewise/latest/appguide/monitor-alarms.html">Monitoring with alarms</a> in the <i>IoT SiteWise Application Guide</i>.
layout: schema
name: Alarms
properties_list:
- description: ''
  name: alarmRoleArn
  type: object
- description: ''
  name: notificationLambdaArn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-alarms-schema.json
slug: iot-sitewise-alarms
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-alarms-schema.json\",\n  \"title\": \"Alarms\",\n  \"description\": \"Contains the configuration information of an alarm created in an IoT SiteWise Monitor portal. You can use the alarm to monitor an asset property and get notified when the asset property value is outside a specified range. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/appguide/monitor-alarms.html\\\">Monitoring with alarms</a> in the <i>IoT SiteWise Application Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alarmRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of\
  \ the IAM role that allows the alarm to perform actions and access Amazon Web Services resources and services, such as IoT Events.\"\n        }\n      ]\n    },\n    \"notificationLambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the Lambda function that manages alarm notifications. For more information, see <a href=\\\"https://docs.aws.amazon.com/iotevents/latest/developerguide/lambda-support.html\\\">Managing alarm notifications</a> in the <i>IoT Events Developer Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"alarmRoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-alarms-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: Alarms
---
