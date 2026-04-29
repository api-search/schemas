---
description: Information about a tool. Tools are used in a simulation job.
layout: schema
name: Tool
properties_list:
- description: ''
  name: streamUI
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: command
  type: object
- description: ''
  name: streamOutputToCloudWatch
  type: object
- description: ''
  name: exitBehavior
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-tool-schema.json
slug: amazon-robomaker-openapi-tool
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-tool-schema.json\",\n  \"title\": \"Tool\",\n  \"description\": \"Information about a tool. Tools are used in a simulation job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"streamUI\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoxedBoolean\"\n        },\n        {\n          \"description\": \"Boolean indicating whether a streaming session will be configured for the tool. If <code>True</code>, AWS RoboMaker will configure a connection so you can interact with the tool as it is running in the simulation. It must have a graphical user interface. The default is <code>False</code>. \"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n \
  \         \"description\": \"The name of the tool.\"\n        }\n      ]\n    },\n    \"command\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UnrestrictedCommand\"\n        },\n        {\n          \"description\": \"Command-line arguments for the tool. It must include the tool executable name.\"\n        }\n      ]\n    },\n    \"streamOutputToCloudWatch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoxedBoolean\"\n        },\n        {\n          \"description\": \"Boolean indicating whether logs will be recorded in CloudWatch for the tool. The default is <code>False</code>. \"\n        }\n      ]\n    },\n    \"exitBehavior\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExitBehavior\"\n        },\n        {\n          \"description\": \"Exit behavior determines what happens when your tool quits running. <code>RESTART</code> will cause your tool to be restarted. <code>FAIL</code> will\
  \ cause your job to exit. The default is <code>RESTART</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"command\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-tool-schema.json
tags:
- AWS
- Robotics
- Simulation
title: Tool
---
