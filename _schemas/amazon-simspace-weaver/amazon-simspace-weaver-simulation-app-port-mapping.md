---
description: A collection of TCP/UDP ports for a custom or service app.
layout: schema
name: SimulationAppPortMapping
properties_list:
- description: ''
  name: Actual
  type: object
- description: ''
  name: Declared
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-simulation-app-port-mapping-schema.json
slug: amazon-simspace-weaver-simulation-app-port-mapping
source_filename: amazon-simspace-weaver-simulation-app-port-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-app-port-mapping-schema.json\",\n  \"title\": \"SimulationAppPortMapping\",\n  \"description\": \"A collection of TCP/UDP ports for a custom or service app.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Actual\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\n        },\n        {\n          \"description\": \"The TCP/UDP port number of the running app. SimSpace Weaver dynamically assigns this port number when the app starts. SimSpace Weaver maps the <code>Declared</code> port to the <code>Actual</code> port. Clients connect to the app using the app's IP address and the <code>Actual</code> port number.\"\n        }\n      ]\n    },\n    \"Declared\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortNumber\"\
  \n        },\n        {\n          \"description\": \"The TCP/UDP port number of the app, declared in the simulation schema. SimSpace Weaver maps the <code>Declared</code> port to the <code>Actual</code> port. The source code for the app should bind to the <code>Declared</code> port.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-simulation-app-port-mapping-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: SimulationAppPortMapping
---
