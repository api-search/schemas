---
description: PutEmailMonitoringConfigurationRequest schema from Amazon WorkMail API
layout: schema
name: PutEmailMonitoringConfigurationRequest
properties_list:
- description: ''
  name: OrganizationId
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: LogGroupArn
  type: object
provider_name: Amazon WorkMail
provider_slug: amazon-workmail
schema_file: json-schema/workmail-put-email-monitoring-configuration-request-schema.json
slug: workmail-put-email-monitoring-configuration-request
source_json: "{\n  \"type\": \"object\",\n  \"required\": [\n    \"OrganizationId\",\n    \"RoleArn\",\n    \"LogGroupArn\"\n  ],\n  \"title\": \"PutEmailMonitoringConfigurationRequest\",\n  \"properties\": {\n    \"OrganizationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationId\"\n        },\n        {\n          \"description\": \"The ID of the organization for which the email monitoring configuration is set.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM Role associated with the email monitoring configuration.\"\n        }\n      ]\n    },\n    \"LogGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the CloudWatch Log group\
  \ associated with the email monitoring configuration.\"\n        }\n      ]\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-email-monitoring-configuration-request-schema.json\",\n  \"description\": \"PutEmailMonitoringConfigurationRequest schema from Amazon WorkMail API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-workmail/refs/heads/main/json-schema/workmail-put-email-monitoring-configuration-request-schema.json
tags:
- AWS
- Business Communication
- Calendar
- Email
- Exchange
- Enterprise
title: PutEmailMonitoringConfigurationRequest
---
