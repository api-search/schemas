---
description: DescribeSimulationApplicationResponse schema from openapi
layout: schema
name: DescribeSimulationApplicationResponse
properties_list:
- description: ''
  name: arn
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: version
  type: object
- description: ''
  name: sources
  type: object
- description: ''
  name: simulationSoftwareSuite
  type: object
- description: ''
  name: robotSoftwareSuite
  type: object
- description: ''
  name: renderingEngine
  type: object
- description: ''
  name: revisionId
  type: object
- description: ''
  name: lastUpdatedAt
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: environment
  type: object
- description: ''
  name: imageDigest
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-describe-simulation-application-response-schema.json
slug: amazon-robomaker-openapi-describe-simulation-application-response
source_filename: amazon-robomaker-openapi-describe-simulation-application-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-application-response-schema.json\",\n  \"title\": \"DescribeSimulationApplicationResponse\",\n  \"description\": \"DescribeSimulationApplicationResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the robot simulation application.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"The name of the simulation application.\"\n        }\n      ]\n    },\n    \"version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/Version\"\n        },\n        {\n          \"description\": \"The version of the simulation application.\"\n        }\n      ]\n    },\n    \"sources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Sources\"\n        },\n        {\n          \"description\": \"The sources of the simulation application.\"\n        }\n      ]\n    },\n    \"simulationSoftwareSuite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationSoftwareSuite\"\n        },\n        {\n          \"description\": \"The simulation software suite used by the simulation application.\"\n        }\n      ]\n    },\n    \"robotSoftwareSuite\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotSoftwareSuite\"\n        },\n        {\n          \"description\": \"Information about the robot software suite (ROS distribution).\"\n        }\n      ]\n    },\n    \"renderingEngine\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/RenderingEngine\"\n        },\n        {\n          \"description\": \"The rendering engine for the simulation application.\"\n        }\n      ]\n    },\n    \"revisionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RevisionId\"\n        },\n        {\n          \"description\": \"The revision id of the simulation application.\"\n        }\n      ]\n    },\n    \"lastUpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedAt\"\n        },\n        {\n          \"description\": \"The time, in milliseconds since the epoch, when the simulation application was last updated.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"The list of all tags added to the specified simulation application.\"\n        }\n      ]\n    },\n    \"\
  environment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Environment\"\n        },\n        {\n          \"description\": \"The object that contains the Docker image URI used to create the simulation application.\"\n        }\n      ]\n    },\n    \"imageDigest\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImageDigest\"\n        },\n        {\n          \"description\": \"A SHA256 identifier for the Docker image that you use for your simulation application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-describe-simulation-application-response-schema.json
tags:
- Robotics
- Simulation
title: DescribeSimulationApplicationResponse
---
