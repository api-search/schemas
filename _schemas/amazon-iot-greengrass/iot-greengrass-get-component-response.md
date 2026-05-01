---
description: GetComponentResponse schema
layout: schema
name: GetComponentResponse
properties_list:
- description: ''
  name: recipeOutputFormat
  type: object
- description: ''
  name: recipe
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-get-component-response-schema.json
slug: iot-greengrass-get-component-response
source_filename: iot-greengrass-get-component-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-component-response-schema.json\",\n  \"title\": \"GetComponentResponse\",\n  \"description\": \"GetComponentResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recipeOutputFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeOutputFormat\"\n        },\n        {\n          \"description\": \"The format of the recipe.\"\n        }\n      ]\n    },\n    \"recipe\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeBlob\"\n        },\n        {\n          \"description\": \"The recipe of the component version.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\":\
  \ \"A list of key-value pairs that contain metadata for the resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/tag-resources.html\\\">Tag your resources</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"recipeOutputFormat\",\n    \"recipe\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-get-component-response-schema.json
tags:
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: GetComponentResponse
---
