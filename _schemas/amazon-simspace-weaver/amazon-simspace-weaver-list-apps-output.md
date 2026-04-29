---
description: ListAppsOutput schema from Amazon SimSpace Weaver API
layout: schema
name: ListAppsOutput
properties_list:
- description: ''
  name: Apps
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-list-apps-output-schema.json
slug: amazon-simspace-weaver-list-apps-output
source_filename: amazon-simspace-weaver-list-apps-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-list-apps-output-schema.json\",\n  \"title\": \"ListAppsOutput\",\n  \"description\": \"ListAppsOutput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Apps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimulationAppList\"\n        },\n        {\n          \"description\": \"The list of apps for the given simulation and domain.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OptionalString\"\n        },\n        {\n          \"description\": \"If SimSpace Weaver returns <code>nextToken</code>, then there are more results available. The value of <code>nextToken</code> is a unique pagination token for each page. To retrieve\
  \ the next page, call the operation again using the returned token. Keep all other arguments unchanged. If no results remain, then <code>nextToken</code> is set to <code>null</code>. Each pagination token expires after 24 hours. If you provide a token that isn't valid, then you receive an <i>HTTP 400 ValidationException</i> error.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-list-apps-output-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: ListAppsOutput
---
