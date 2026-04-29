---
description: CreateComponentVersionRequest schema
layout: schema
name: CreateComponentVersionRequest
properties_list:
- description: ''
  name: inlineRecipe
  type: object
- description: ''
  name: lambdaFunction
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-create-component-version-request-schema.json
slug: iot-greengrass-create-component-version-request
source_filename: iot-greengrass-create-component-version-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-component-version-request-schema.json\",\n  \"title\": \"CreateComponentVersionRequest\",\n  \"description\": \"CreateComponentVersionRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inlineRecipe\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecipeBlob\"\n        },\n        {\n          \"description\": \"<p>The recipe to use to create the component. The recipe defines the component's metadata, parameters, dependencies, lifecycle, artifacts, and platform compatibility.</p> <p>You must specify either <code>inlineRecipe</code> or <code>lambdaFunction</code>.</p>\"\n        }\n      ]\n    },\n    \"lambdaFunction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaFunctionRecipeSource\"\n\
  \        },\n        {\n          \"description\": \"<p>The parameters to create a component from a Lambda function.</p> <p>You must specify either <code>inlineRecipe</code> or <code>lambdaFunction</code>.</p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of key-value pairs that contain metadata for the resource. For more information, see <a href=\\\"https://docs.aws.amazon.com/greengrass/v2/developerguide/tag-resources.html\\\">Tag your resources</a> in the <i>IoT Greengrass V2 Developer Guide</i>.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientTokenString\"\n        },\n        {\n          \"description\": \"A unique, case-sensitive identifier that you can provide to ensure that the request is idempotent. Idempotency means that the request is successfully\
  \ processed only once, even if you send the request multiple times. When a request succeeds, and you specify the same client token for subsequent successful requests, the IoT Greengrass V2 service returns the successful response that it caches from the previous request. IoT Greengrass V2 caches successful responses for idempotent requests for up to 8 hours.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-create-component-version-request-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: CreateComponentVersionRequest
---
