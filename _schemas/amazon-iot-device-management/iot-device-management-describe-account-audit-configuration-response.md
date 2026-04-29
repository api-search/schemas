---
description: DescribeAccountAuditConfigurationResponse schema
layout: schema
name: DescribeAccountAuditConfigurationResponse
properties_list:
- description: ''
  name: roleArn
  type: object
- description: ''
  name: auditNotificationTargetConfigurations
  type: object
- description: ''
  name: auditCheckConfigurations
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-account-audit-configuration-response-schema.json
slug: iot-device-management-describe-account-audit-configuration-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-account-audit-configuration-response-schema.json\",\n  \"title\": \"DescribeAccountAuditConfigurationResponse\",\n  \"description\": \"DescribeAccountAuditConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"<p>The ARN of the role that grants permission to IoT to access information about your devices, policies, certificates, and other items as required when performing an audit.</p> <p>On the first call to <code>UpdateAccountAuditConfiguration</code>, this parameter is required.</p>\"\n        }\n      ]\n    },\n    \"auditNotificationTargetConfigurations\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/AuditNotificationTargetConfigurations\"\n        },\n        {\n          \"description\": \"Information about the targets to which audit notifications are sent for this account.\"\n        }\n      ]\n    },\n    \"auditCheckConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuditCheckConfigurations\"\n        },\n        {\n          \"description\": \"Which audit checks are enabled and disabled for this account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-account-audit-configuration-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeAccountAuditConfigurationResponse
---
