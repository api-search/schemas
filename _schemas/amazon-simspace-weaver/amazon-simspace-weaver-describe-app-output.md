---
description: DescribeAppOutput schema from Amazon SimSpace Weaver API
layout: schema
name: DescribeAppOutput
properties_list:
- description: ''
  name: Description
  type: object
- description: ''
  name: Domain
  type: object
- description: ''
  name: EndpointInfo
  type: object
- description: ''
  name: LaunchOverrides
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
schema_file: json-schema/amazon-simspace-weaver-describe-app-output-schema.json
slug: amazon-simspace-weaver-describe-app-output
source_filename: amazon-simspace-weaver-describe-app-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-describe-app-output-schema.json\",\n  \"title\": \"DescribeAppOutput\",\n  \"description\": \"DescribeAppOutput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n        {\n          \"description\": \"The description of the app.\"\n        }\n      ]\n    },\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the domain of the app.\"\n        }\n      ]\n    },\n    \"EndpointInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationAppEndpointInfo\"\
  \n        },\n        {\n          \"description\": \"Information about the network endpoint for the custom app. You can use the endpoint to connect to the custom app.\"\n        }\n      ]\n    },\n    \"LaunchOverrides\": {\n      \"$ref\": \"#/components/schemas/LaunchOverrides\"\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverLongResourceName\"\n        },\n        {\n          \"description\": \"The name of the app.\"\n        }\n      ]\n    },\n    \"Simulation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the simulation of the app.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationAppStatus\"\n        },\n        {\n          \"description\": \"The current lifecycle state of the custom app.\"\n        }\n\
  \      ]\n    },\n    \"TargetStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationAppTargetStatus\"\n        },\n        {\n          \"description\": \"The desired lifecycle state of the custom app.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-describe-app-output-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: DescribeAppOutput
---
