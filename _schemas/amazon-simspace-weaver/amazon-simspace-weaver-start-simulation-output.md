---
description: StartSimulationOutput schema from Amazon SimSpace Weaver API
layout: schema
name: StartSimulationOutput
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ExecutionId
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-start-simulation-output-schema.json
slug: amazon-simspace-weaver-start-simulation-output
source_filename: amazon-simspace-weaver-start-simulation-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-simulation-output-schema.json\",\n  \"title\": \"StartSimulationOutput\",\n  \"description\": \"StartSimulationOutput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the simulation. For more information about ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n\
  \        },\n        {\n          \"description\": \"The time when the simulation was created, expressed as the number of seconds and milliseconds in UTC since the Unix epoch (0:0:0.000, January 1, 1970).\"\n        }\n      ]\n    },\n    \"ExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UUID\"\n        },\n        {\n          \"description\": \"A universally unique identifier (UUID) for this simulation.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-simulation-output-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: StartSimulationOutput
---
