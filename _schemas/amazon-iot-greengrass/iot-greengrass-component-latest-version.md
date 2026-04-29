---
description: Contains information about the latest version of a component.
layout: schema
name: ComponentLatestVersion
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: componentVersion
  type: object
- description: ''
  name: creationTimestamp
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: publisher
  type: object
- description: ''
  name: platforms
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-latest-version-schema.json
slug: iot-greengrass-component-latest-version
source_filename: iot-greengrass-component-latest-version-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-latest-version-schema.json\",\n  \"title\": \"ComponentLatestVersion\",\n  \"description\": \"Contains information about the latest version of a component.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the component version.\"\n        }\n      ]\n    },\n    \"componentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionString\"\n        },\n        {\n          \"description\": \"The version of the component.\"\n        }\n      ]\n    },\n    \"creationTimestamp\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the component was created, expressed in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The description of the component version.\"\n        }\n      ]\n    },\n    \"publisher\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The publisher of the component version.\"\n        }\n      ]\n    },\n    \"platforms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentPlatformList\"\n        },\n        {\n          \"description\": \"The platforms that the component version supports.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-latest-version-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentLatestVersion
---
