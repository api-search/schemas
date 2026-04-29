---
description: DescribeProvisioningTemplateResponse schema
layout: schema
name: DescribeProvisioningTemplateResponse
properties_list:
- description: ''
  name: templateArn
  type: object
- description: ''
  name: templateName
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: creationDate
  type: object
- description: ''
  name: lastModifiedDate
  type: object
- description: ''
  name: defaultVersionId
  type: object
- description: ''
  name: templateBody
  type: object
- description: ''
  name: enabled
  type: object
- description: ''
  name: provisioningRoleArn
  type: object
- description: ''
  name: preProvisioningHook
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon IoT Device Management
provider_slug: amazon-iot-device-management
schema_file: json-schema/iot-device-management-describe-provisioning-template-response-schema.json
slug: iot-device-management-describe-provisioning-template-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-provisioning-template-response-schema.json\",\n  \"title\": \"DescribeProvisioningTemplateResponse\",\n  \"description\": \"DescribeProvisioningTemplateResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"templateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateArn\"\n        },\n        {\n          \"description\": \"The ARN of the provisioning template.\"\n        }\n      ]\n    },\n    \"templateName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateName\"\n        },\n        {\n          \"description\": \"The name of the provisioning template.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateDescription\"\
  \n        },\n        {\n          \"description\": \"The description of the provisioning template.\"\n        }\n      ]\n    },\n    \"creationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date when the provisioning template was created.\"\n        }\n      ]\n    },\n    \"lastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateType\"\n        },\n        {\n          \"description\": \"The date when the provisioning template was last modified.\"\n        }\n      ]\n    },\n    \"defaultVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateVersionId\"\n        },\n        {\n          \"description\": \"The default fleet template version ID.\"\n        }\n      ]\n    },\n    \"templateBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateBody\"\n   \
  \     },\n        {\n          \"description\": \"The JSON formatted contents of the provisioning template.\"\n        }\n      ]\n    },\n    \"enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Enabled\"\n        },\n        {\n          \"description\": \"True if the provisioning template is enabled, otherwise false.\"\n        }\n      ]\n    },\n    \"provisioningRoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the role associated with the provisioning template. This IoT role grants permission to provision a device.\"\n        }\n      ]\n    },\n    \"preProvisioningHook\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ProvisioningHook\"\n        },\n        {\n          \"description\": \"Gets information about a pre-provisioned hook.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/TemplateType\"\n        },\n        {\n          \"description\": \"The type you define in a provisioning template. You can create a template with only one type. You can't change the template type after its creation. The default value is <code>FLEET_PROVISIONING</code>. For more information about provisioning template, see: <a href=\\\"https://docs.aws.amazon.com/iot/latest/developerguide/provision-template.html\\\">Provisioning template</a>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-device-management/refs/heads/main/json-schema/iot-device-management-describe-provisioning-template-response-schema.json
tags:
- AWS
- Device Management
- Fleet Management
- IoT
- OTA Updates
title: DescribeProvisioningTemplateResponse
---
