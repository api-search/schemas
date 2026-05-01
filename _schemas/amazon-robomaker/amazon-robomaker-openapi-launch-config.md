---
description: Information about a launch configuration.
layout: schema
name: LaunchConfig
properties_list:
- description: ''
  name: packageName
  type: object
- description: ''
  name: launchFile
  type: object
- description: ''
  name: environmentVariables
  type: object
- description: ''
  name: portForwardingConfig
  type: object
- description: ''
  name: streamUI
  type: object
- description: ''
  name: command
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-launch-config-schema.json
slug: amazon-robomaker-openapi-launch-config
source_filename: amazon-robomaker-openapi-launch-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-launch-config-schema.json\",\n  \"title\": \"LaunchConfig\",\n  \"description\": \"Information about a launch configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Command\"\n        },\n        {\n          \"description\": \"The package name.\"\n        }\n      ]\n    },\n    \"launchFile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Command\"\n        },\n        {\n          \"description\": \"The launch file name.\"\n        }\n      ]\n    },\n    \"environmentVariables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EnvironmentVariableMap\"\n        },\n        {\n          \"description\": \"The\
  \ environment variables for the application launch.\"\n        }\n      ]\n    },\n    \"portForwardingConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortForwardingConfig\"\n        },\n        {\n          \"description\": \"The port forwarding configuration.\"\n        }\n      ]\n    },\n    \"streamUI\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Boolean indicating whether a streaming session will be configured for the application. If <code>True</code>, AWS RoboMaker will configure a connection so you can interact with your application as it is running in the simulation. You must configure and launch the component. It must have a graphical user interface. \"\n        }\n      ]\n    },\n    \"command\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CommandList\"\n        },\n        {\n          \"description\": \"<p>If\
  \ you've specified <code>General</code> as the value for your <code>RobotSoftwareSuite</code>, you can use this field to specify a list of commands for your container image.</p> <p>If you've specified <code>SimulationRuntime</code> as the value for your <code>SimulationSoftwareSuite</code>, you can use this field to specify a list of commands for your container image.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-launch-config-schema.json
tags:
- Robotics
- Simulation
title: LaunchConfig
---
