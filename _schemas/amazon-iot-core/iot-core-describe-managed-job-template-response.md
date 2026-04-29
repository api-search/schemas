---
description: DescribeManagedJobTemplateResponse schema
layout: schema
name: DescribeManagedJobTemplateResponse
properties_list:
- description: ''
  name: templateName
  type: object
- description: ''
  name: templateArn
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: templateVersion
  type: object
- description: ''
  name: environments
  type: object
- description: ''
  name: documentParameters
  type: object
- description: ''
  name: document
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-describe-managed-job-template-response-schema.json
slug: iot-core-describe-managed-job-template-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-managed-job-template-response-schema.json\",\n  \"title\": \"DescribeManagedJobTemplateResponse\",\n  \"description\": \"DescribeManagedJobTemplateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagedJobTemplateName\"\n        },\n        {\n          \"description\": \"The unique name of a managed template, such as <code>AWS-Reboot</code>.\"\n        }\n      ]\n    },\n    \"templateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobTemplateArn\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) of the managed template.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/JobDescription\"\n        },\n        {\n          \"description\": \"The unique description of a managed template.\"\n        }\n      ]\n    },\n    \"templateVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ManagedTemplateVersion\"\n        },\n        {\n          \"description\": \"The version for a managed template.\"\n        }\n      ]\n    },\n    \"environments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Environments\"\n        },\n        {\n          \"description\": \"A list of environments that are supported with the managed job template.\"\n        }\n      ]\n    },\n    \"documentParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DocumentParameters\"\n        },\n        {\n          \"description\": \"<p>A map of key-value pairs that you can use as guidance to specify the inputs for creating a job\
  \ from a managed template.</p> <note> <p> <code>documentParameters</code> can only be used when creating jobs from Amazon Web Services managed templates. This parameter can't be used with custom job templates or to create jobs from them.</p> </note>\"\n        }\n      ]\n    },\n    \"document\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobDocument\"\n        },\n        {\n          \"description\": \"The document schema for a managed job template.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-describe-managed-job-template-response-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: DescribeManagedJobTemplateResponse
---
