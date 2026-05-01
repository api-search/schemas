---
description: StartAppOutput schema from Amazon SimSpace Weaver API
layout: schema
name: StartAppOutput
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
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-start-app-output-schema.json
slug: amazon-simspace-weaver-start-app-output
source_filename: amazon-simspace-weaver-start-app-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-app-output-schema.json\",\n  \"title\": \"StartAppOutput\",\n  \"description\": \"StartAppOutput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the domain of the app.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the app.\"\n        }\n      ]\n    },\n    \"Simulation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\
  \n        },\n        {\n          \"description\": \"The name of the simulation of the app.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-app-output-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: StartAppOutput
---
