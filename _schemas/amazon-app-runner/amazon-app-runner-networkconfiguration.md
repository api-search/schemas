---
description: Describes configuration settings related to network traffic of an App Runner service. Consists of embedded objects for each configurable network feature.
layout: schema
name: NetworkConfiguration
properties_list:
- description: ''
  name: EgressConfiguration
  type: object
- description: ''
  name: IngressConfiguration
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-networkconfiguration-schema.json
slug: amazon-app-runner-networkconfiguration
source_filename: amazon-app-runner-networkconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"NetworkConfiguration\",\n  \"description\": \"Describes configuration settings related to network traffic of an App Runner service. Consists of embedded objects for each configurable network feature.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EgressConfiguration\": {},\n    \"IngressConfiguration\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-networkconfiguration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: NetworkConfiguration
---
