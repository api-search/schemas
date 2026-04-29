---
description: Information about a deployment application configuration.
layout: schema
name: DeploymentApplicationConfig
properties_list:
- description: ''
  name: application
  type: object
- description: ''
  name: applicationVersion
  type: object
- description: ''
  name: launchConfig
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-deployment-application-config-schema.json
slug: amazon-robomaker-openapi-deployment-application-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deployment-application-config-schema.json\",\n  \"title\": \"DeploymentApplicationConfig\",\n  \"description\": \"Information about a deployment application configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the robot application.\"\n        }\n      ]\n    },\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeploymentVersion\"\n        },\n        {\n          \"description\": \"The version of the application.\"\n        }\n      ]\n    },\n    \"launchConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/DeploymentLaunchConfig\"\n        },\n        {\n          \"description\": \"The launch configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"application\",\n    \"applicationVersion\",\n    \"launchConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-deployment-application-config-schema.json
tags:
- AWS
- Robotics
- Simulation
title: DeploymentApplicationConfig
---
