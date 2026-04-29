---
description: A collection of metadata about the app.
layout: schema
name: SimulationAppMetadata
properties_list:
- description: ''
  name: Domain
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Simulation
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: TargetStatus
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-simulation-app-metadata-schema.json
slug: amazon-simspace-weaver-simulation-app-metadata
source_filename: amazon-simspace-weaver-simulation-app-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-app-metadata-schema.json\",\n  \"title\": \"SimulationAppMetadata\",\n  \"description\": \"A collection of metadata about the app.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The domain of the app. For more information about domains, see <a href=\\\"https://docs.aws.amazon.com/simspaceweaver/latest/userguide/what-is_key-concepts.html#what-is_key-concepts_domains\\\">Key concepts: Domains</a> in the <i>SimSpace Weaver User Guide</i>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverLongResourceName\"\
  \n        },\n        {\n          \"description\": \"The name of the app.\"\n        }\n      ]\n    },\n    \"Simulation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the simulation of the app.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationAppStatus\"\n        },\n        {\n          \"description\": \"The current status of the app.\"\n        }\n      ]\n    },\n    \"TargetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationAppTargetStatus\"\n        },\n        {\n          \"description\": \"The desired status of the app.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-app-metadata-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: SimulationAppMetadata
---
