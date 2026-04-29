---
description: CreateProvisioningTemplateResponse schema
layout: schema
name: CreateProvisioningTemplateResponse
properties_list:
- description: ''
  name: templateArn
  type: object
- description: ''
  name: templateName
  type: object
- description: ''
  name: defaultVersionId
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-create-provisioning-template-response-schema.json
slug: iot-device-defender-create-provisioning-template-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-provisioning-template-response-schema.json\",\n  \"title\": \"CreateProvisioningTemplateResponse\",\n  \"description\": \"CreateProvisioningTemplateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateArn\"\n        },\n        {\n          \"description\": \"The ARN that identifies the provisioning template.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateName\"\n        },\n        {\n          \"description\": \"The name of the provisioning template.\"\n        }\n      ]\n    },\n    \"defaultVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/TemplateVersionId\"\n        },\n        {\n          \"description\": \"The default version of the provisioning template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-create-provisioning-template-response-schema.json
tags:
- AWS
- Compliance
- IoT
- Security
- Vulnerability Management
title: CreateProvisioningTemplateResponse
---
