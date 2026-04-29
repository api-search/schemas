---
description: ComponentList schema
layout: schema
name: ComponentList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-list-schema.json
slug: iot-greengrass-component-list
source_filename: iot-greengrass-component-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-list-schema.json\",\n  \"title\": \"ComponentList\",\n  \"description\": \"ComponentList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"arn\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentARN\"\n          },\n          {\n            \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the component version.\"\n          }\n        ]\n      },\n      \"componentName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentNameString\"\n          },\n          {\n            \"description\": \"The name of the component.\"\n          }\n        ]\n      },\n\
  \      \"latestVersion\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentLatestVersion\"\n          },\n          {\n            \"description\": \"The latest version of the component and its details.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a component.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentList
---
