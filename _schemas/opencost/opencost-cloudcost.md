---
description: ''
layout: schema
name: OpenCost CloudCost
properties_list:
- description: ''
  name: netCost
  type: object
provider_name: OpenCost
provider_slug: opencost
schema_file: json-schema/opencost-cloudcost-schema.json
slug: opencost-cloudcost
source_filename: opencost-cloudcost-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/opencost/json-schema/opencost-cloudcost-schema.json\",\n  \"title\": \"OpenCost CloudCost\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"netCost\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cost\": {\"type\": \"number\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/opencost/refs/heads/main/json-schema/opencost-cloudcost-schema.json
tags:
- Cloud Cost Management
- CNCF
- FinOps
- Kubernetes
- Observability
title: OpenCost CloudCost
---
