---
description: 'Information about the network endpoint that you can use to connect to your custom or service app. For more information about SimSpace Weaver apps, see <a href="https://docs.aws.amazon.com/simspaceweaver/latest/userguide/what-is_key-concepts.html#what-is_key-concepts_apps">Key concepts: Apps</a> in the <i>SimSpace Weaver User Guide</i>..'
layout: schema
name: SimulationAppEndpointInfo
properties_list:
- description: ''
  name: Address
  type: object
- description: ''
  name: IngressPortMappings
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-simulation-app-endpoint-info-schema.json
slug: amazon-simspace-weaver-simulation-app-endpoint-info
source_filename: amazon-simspace-weaver-simulation-app-endpoint-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-app-endpoint-info-schema.json\",\n  \"title\": \"SimulationAppEndpointInfo\",\n  \"description\": \"Information about the network endpoint that you can use to connect to your custom or service app. For more information about SimSpace Weaver apps, see <a href=\\\"https://docs.aws.amazon.com/simspaceweaver/latest/userguide/what-is_key-concepts.html#what-is_key-concepts_apps\\\">Key concepts: Apps</a> in the <i>SimSpace Weaver User Guide</i>..\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Address\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The IP address of the app. SimSpace Weaver dynamically assigns this IP address when the app starts.\"\n        }\n\
  \      ]\n    },\n    \"IngressPortMappings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AppPortMappings\"\n        },\n        {\n          \"description\": \"The inbound TCP/UDP port numbers of the app. The combination of an IP address and a port number form a network endpoint.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-app-endpoint-info-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: SimulationAppEndpointInfo
---
