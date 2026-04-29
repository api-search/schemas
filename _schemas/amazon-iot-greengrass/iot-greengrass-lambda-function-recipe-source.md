---
description: Contains information about an Lambda function to import to create a component.
layout: schema
name: LambdaFunctionRecipeSource
properties_list:
- description: ''
  name: lambdaArn
  type: object
- description: ''
  name: componentName
  type: object
- description: ''
  name: componentVersion
  type: object
- description: ''
  name: componentPlatforms
  type: object
- description: ''
  name: componentDependencies
  type: object
- description: ''
  name: componentLambdaParameters
  type: object
provider_name: Amazon IoT Greengrass
provider_slug: amazon-iot-greengrass
schema_file: json-schema/iot-greengrass-lambda-function-recipe-source-schema.json
slug: iot-greengrass-lambda-function-recipe-source
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-function-recipe-source-schema.json\",\n  \"title\": \"LambdaFunctionRecipeSource\",\n  \"description\": \"Contains information about an Lambda function to import to create a component.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the Lambda function. The ARN must include the version of the function to import. You can't use version aliases like <code>$LATEST</code>.\"\n        }\n      ]\n    },\n    \"componentName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentNameString\"\
  \n        },\n        {\n          \"description\": \"<p>The name of the component.</p> <p>Defaults to the name of the Lambda function.</p>\"\n        }\n      ]\n    },\n    \"componentVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentVersionString\"\n        },\n        {\n          \"description\": \"<p>The version of the component.</p> <p>Defaults to the version of the Lambda function as a semantic version. For example, if your function version is <code>3</code>, the component version becomes <code>3.0.0</code>.</p>\"\n        }\n      ]\n    },\n    \"componentPlatforms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentPlatformList\"\n        },\n        {\n          \"description\": \"The platforms that the component version supports.\"\n        }\n      ]\n    },\n    \"componentDependencies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComponentDependencyMap\"\
  \n        },\n        {\n          \"description\": \"The component versions on which this Lambda function component depends.\"\n        }\n      ]\n    },\n    \"componentLambdaParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaExecutionParameters\"\n        },\n        {\n          \"description\": \"The system and runtime parameters for the Lambda function as it runs on the Greengrass core device.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"lambdaArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-greengrass/refs/heads/main/json-schema/iot-greengrass-lambda-function-recipe-source-schema.json
tags:
- AWS
- Edge Computing
- IoT
- Lambda
- Machine Learning
- Real-Time Processing
title: LambdaFunctionRecipeSource
---
