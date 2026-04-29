---
description: The logging configuration for a simulation.
layout: schema
name: LoggingConfiguration
properties_list:
- description: ''
  name: Destinations
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-logging-configuration-schema.json
slug: amazon-simspace-weaver-logging-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-logging-configuration-schema.json\",\n  \"title\": \"LoggingConfiguration\",\n  \"description\": \"The logging configuration for a simulation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destinations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogDestinations\"\n        },\n        {\n          \"description\": \"A list of the locations where SimSpace Weaver sends simulation log data.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-logging-configuration-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: LoggingConfiguration
---
