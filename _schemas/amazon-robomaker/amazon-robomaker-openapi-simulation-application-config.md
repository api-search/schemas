---
description: Information about a simulation application configuration.
layout: schema
name: SimulationApplicationConfig
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
- description: ''
  name: uploadConfigurations
  type: object
- description: ''
  name: worldConfigs
  type: object
- description: ''
  name: useDefaultUploadConfigurations
  type: object
- description: ''
  name: tools
  type: object
- description: ''
  name: useDefaultTools
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-simulation-application-config-schema.json
slug: amazon-robomaker-openapi-simulation-application-config
source_filename: amazon-robomaker-openapi-simulation-application-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-application-config-schema.json\",\n  \"title\": \"SimulationApplicationConfig\",\n  \"description\": \"Information about a simulation application configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The application information for the simulation application.\"\n        }\n      ]\n    },\n    \"applicationVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the simulation application.\"\n        }\n      ]\n    },\n    \"launchConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/LaunchConfig\"\n        },\n        {\n          \"description\": \"The launch configuration for the simulation application.\"\n        }\n      ]\n    },\n    \"uploadConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UploadConfigurations\"\n        },\n        {\n          \"description\": \"Information about upload configurations for the simulation application.\"\n        }\n      ]\n    },\n    \"worldConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorldConfigs\"\n        },\n        {\n          \"description\": \"A list of world configurations.\"\n        }\n      ]\n    },\n    \"useDefaultUploadConfigurations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoxedBoolean\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"<p>A Boolean indicating whether to use default upload configurations. By default, <code>.ros</code>\
  \ and <code>.gazebo</code> files are uploaded when the application terminates and all ROS topics will be recorded.</p> <p>If you set this value, you must specify an <code>outputLocation</code>.</p> <important> <p>This API is no longer supported and will throw an error if used.</p> </important>AWS RoboMaker is ending support for ROS software suite. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/software-support-policy.html.\"\n        }\n      ]\n    },\n    \"tools\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tools\"\n        },\n        {\n          \"description\": \"Information about tools configured for the simulation application.\"\n        }\n      ]\n    },\n    \"useDefaultTools\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BoxedBoolean\"\n        },\n        {\n          \"deprecated\": true,\n          \"description\": \"<p>A Boolean indicating whether to use default simulation\
  \ application tools. The default tools are rviz, rqt, terminal and rosbag record. The default is <code>False</code>.</p> <important> <p>This API is no longer supported and will throw an error if used.</p> </important>AWS RoboMaker is ending support for ROS software suite. For additional information, see https://docs.aws.amazon.com/robomaker/latest/dg/software-support-policy.html.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"application\",\n    \"launchConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-simulation-application-config-schema.json
tags:
- Robotics
- Simulation
title: SimulationApplicationConfig
---
