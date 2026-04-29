---
description: CreateProvisioningTemplateVersionResponse schema
layout: schema
name: CreateProvisioningTemplateVersionResponse
properties_list:
- description: ''
  name: templateArn
  type: object
- description: ''
  name: templateName
  type: object
- description: ''
  name: versionId
  type: object
- description: ''
  name: isDefaultVersion
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-provisioning-template-version-response-schema.json
slug: iot-device-defender-create-provisioning-template-version-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-provisioning-template-version-response-schema.json\",\n  \"title\": \"CreateProvisioningTemplateVersionResponse\",\n  \"description\": \"CreateProvisioningTemplateVersionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateArn\"\n        },\n        {\n          \"description\": \"The ARN that identifies the provisioning template.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateName\"\n        },\n        {\n          \"description\": \"The name of the provisioning template.\"\n        }\n      ]\n    },\n    \"versionId\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/TemplateVersionId\"\n        },\n        {\n          \"description\": \"The version of the provisioning template.\"\n        }\n      ]\n    },\n    \"isDefaultVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsDefaultVersion\"\n        },\n        {\n          \"description\": \"True if the provisioning template version is the default version, otherwise false.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-provisioning-template-version-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateProvisioningTemplateVersionResponse
---
