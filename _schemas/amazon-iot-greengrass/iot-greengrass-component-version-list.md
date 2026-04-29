---
description: ComponentVersionList schema
layout: schema
name: ComponentVersionList
properties_list: []
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-component-version-list-schema.json
slug: iot-greengrass-component-version-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-version-list-schema.json\",\n  \"title\": \"ComponentVersionList\",\n  \"description\": \"ComponentVersionList schema\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"componentName\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentNameString\"\n          },\n          {\n            \"description\": \"The name of the component.\"\n          }\n        ]\n      },\n      \"componentVersion\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/ComponentVersionString\"\n          },\n          {\n            \"description\": \"The version of the component.\"\n          }\n        ]\n      },\n      \"arn\": {\n        \"allOf\": [\n          {\n \
  \           \"$ref\": \"#/components/schemas/NonEmptyString\"\n          },\n          {\n            \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the component version.\"\n          }\n        ]\n      }\n    },\n    \"description\": \"Contains information about a component version in a list.\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-component-version-list-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: ComponentVersionList
---
