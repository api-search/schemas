---
description: A collection of additional state information, such as domain and clock configuration.
layout: schema
name: LiveSimulationState
properties_list:
- description: ''
  name: Clocks
  type: object
- description: ''
  name: Domains
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-live-simulation-state-schema.json
slug: amazon-simspace-weaver-live-simulation-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-live-simulation-state-schema.json\",\n  \"title\": \"LiveSimulationState\",\n  \"description\": \"A collection of additional state information, such as domain and clock configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Clocks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationClockList\"\n        },\n        {\n          \"description\": \"<p>A list of simulation clocks.</p> <note> <p>At this time, a simulation has only one clock.</p> </note>\"\n        }\n      ]\n    },\n    \"Domains\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainList\"\n        },\n        {\n          \"description\": \"A list of domains for the simulation. For more information about domains, see <a href=\\\
  \"https://docs.aws.amazon.com/simspaceweaver/latest/userguide/what-is_key-concepts.html#what-is_key-concepts_domains\\\">Key concepts: Domains</a> in the <i>SimSpace Weaver User Guide</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-live-simulation-state-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: LiveSimulationState
---
