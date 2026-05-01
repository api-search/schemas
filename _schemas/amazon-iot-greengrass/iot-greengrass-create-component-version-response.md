---
description: CreateComponentVersionResponse schema
layout: schema
name: CreateComponentVersionResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: componentName
  type: object
- description: ''
  name: componentVersion
  type: object
- description: ''
  name: creationTimestamp
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-create-component-version-response-schema.json
slug: iot-greengrass-create-component-version-response
source_filename: iot-greengrass-create-component-version-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-component-version-response-schema.json\",\n  \"title\": \"CreateComponentVersionResponse\",\n  \"description\": \"CreateComponentVersionResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the component version.\"\n        }\n      ]\n    },\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentNameString\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n        }\n      ]\n    },\n    \"componentVersion\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionString\"\n        },\n        {\n          \"description\": \"The version of the component.\"\n        }\n      ]\n    },\n    \"creationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the component was created, expressed in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudComponentStatus\"\n        },\n        {\n          \"description\": \"The status of the component version in IoT Greengrass V2. This status is different from the status of the component on a core device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"componentName\",\n    \"componentVersion\",\n    \"creationTimestamp\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-component-version-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: CreateComponentVersionResponse
---
