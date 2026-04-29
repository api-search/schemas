---
description: ListSimulationsOutput schema from Amazon SimSpace Weaver API
layout: schema
name: ListSimulationsOutput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: Simulations
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-list-simulations-output-schema.json
slug: amazon-simspace-weaver-list-simulations-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-list-simulations-output-schema.json\",\n  \"title\": \"ListSimulationsOutput\",\n  \"description\": \"ListSimulationsOutput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalString\"\n        },\n        {\n          \"description\": \"If SimSpace Weaver returns <code>nextToken</code>, then there are more results available. The value of <code>nextToken</code> is a unique pagination token for each page. To retrieve the next page, call the operation again using the returned token. Keep all other arguments unchanged. If no results remain, then <code>nextToken</code> is set to <code>null</code>. Each pagination token expires after 24 hours.\
  \ If you provide a token that isn't valid, then you receive an <i>HTTP 400 ValidationException</i> error.\"\n        }\n      ]\n    },\n    \"Simulations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationList\"\n        },\n        {\n          \"description\": \"The list of simulations.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-list-simulations-output-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: ListSimulationsOutput
---
