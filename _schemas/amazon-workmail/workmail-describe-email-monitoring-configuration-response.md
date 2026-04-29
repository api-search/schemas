---
description: DescribeEmailMonitoringConfigurationResponse schema from Amazon WorkMail API
layout: schema
name: DescribeEmailMonitoringConfigurationResponse
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: LogGroupArn
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-describe-email-monitoring-configuration-response-schema.json
slug: workmail-describe-email-monitoring-configuration-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM Role associated with the email monitoring configuration.\"\n        }\n      ]\n    },\n    \"LogGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the CloudWatch Log group associated with the email monitoring configuration.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeEmailMonitoringConfigurationResponse\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-email-monitoring-configuration-response-schema.json\",\n  \"description\": \"DescribeEmailMonitoringConfigurationResponse\
  \ schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-describe-email-monitoring-configuration-response-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: DescribeEmailMonitoringConfigurationResponse
---
