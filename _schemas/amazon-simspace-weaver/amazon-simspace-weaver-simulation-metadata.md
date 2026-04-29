---
description: A collection of data about the simulation.
layout: schema
name: SimulationMetadata
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: TargetStatus
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-simulation-metadata-schema.json
slug: amazon-simspace-weaver-simulation-metadata
source_filename: amazon-simspace-weaver-simulation-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-metadata-schema.json\",\n  \"title\": \"SimulationMetadata\",\n  \"description\": \"A collection of data about the simulation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the simulation. For more information about ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n \
  \         \"description\": \"The time when the simulation was created, expressed as the number of seconds and milliseconds in UTC since the Unix epoch (0:0:0.000, January 1, 1970).\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the simulation.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationStatus\"\n        },\n        {\n          \"description\": \"The current status of the simulation.\"\n        }\n      ]\n    },\n    \"TargetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationTargetStatus\"\n        },\n        {\n          \"description\": \"The desired status of the simulation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-metadata-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: SimulationMetadata
---
