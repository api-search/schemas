---
description: DescribeProvisioningTemplateVersionResponse schema
layout: schema
name: DescribeProvisioningTemplateVersionResponse
properties_list:
- description: ''
  name: versionId
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: templateBody
  type: object
- description: ''
  name: isDefaultVersion
  type: object
provider_name: Amazon IoT Device Defender
provider_slug: amazon-iot-device-defender
schema_file: json-schema/iot-device-defender-describe-provisioning-template-version-response-schema.json
slug: iot-device-defender-describe-provisioning-template-version-response
source_filename: iot-device-defender-describe-provisioning-template-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-provisioning-template-version-response-schema.json\",\n  \"title\": \"DescribeProvisioningTemplateVersionResponse\",\n  \"description\": \"DescribeProvisioningTemplateVersionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionId\"\n        },\n        {\n          \"description\": \"The provisioning template version ID.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date when the provisioning template version was created.\"\n        }\n      ]\n    },\n    \"templateBody\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/TemplateBody\"\n        },\n        {\n          \"description\": \"The JSON formatted contents of the provisioning template version.\"\n        }\n      ]\n    },\n    \"isDefaultVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IsDefaultVersion\"\n        },\n        {\n          \"description\": \"True if the provisioning template version is the default version.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-defender/refs/heads/main/json-schema/iot-device-defender-describe-provisioning-template-version-response-schema.json
tags:
- Compliance
- IoT
- Security
- Vulnerability Management
title: DescribeProvisioningTemplateVersionResponse
---
