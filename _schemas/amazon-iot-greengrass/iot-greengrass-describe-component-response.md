---
description: DescribeComponentResponse schema
layout: schema
name: DescribeComponentResponse
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
  name: publisher
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: platforms
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-describe-component-response-schema.json
slug: iot-greengrass-describe-component-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-describe-component-response-schema.json\",\n  \"title\": \"DescribeComponentResponse\",\n  \"description\": \"DescribeComponentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionARN\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the component version.\"\n        }\n      ]\n    },\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentNameString\"\n        },\n        {\n          \"description\": \"The name of the component.\"\n        }\n      ]\n    },\n    \"componentVersion\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionString\"\n        },\n        {\n          \"description\": \"The version of the component.\"\n        }\n      ]\n    },\n    \"creationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the component was created, expressed in ISO 8601 format.\"\n        }\n      ]\n    },\n    \"publisher\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PublisherString\"\n        },\n        {\n          \"description\": \"The publisher of the component version.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescriptionString\"\n        },\n        {\n          \"description\": \"The description of the component version.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/CloudComponentStatus\"\n        },\n        {\n          \"description\": \"The status of the component version in IoT Greengrass V2. This status is different from the status of the component on a core device.\"\n        }\n      ]\n    },\n    \"platforms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentPlatformList\"\n        },\n        {\n          \"description\": \"The platforms that the component version supports.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of key-value pairs that contain metadata for the resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/tag-resources.html\\\">Tag your resources</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-describe-component-response-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: DescribeComponentResponse
---
