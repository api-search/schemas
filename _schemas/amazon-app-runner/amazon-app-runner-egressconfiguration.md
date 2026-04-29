---
description: Describes configuration settings related to outbound network traffic of an App Runner service.
layout: schema
name: EgressConfiguration
properties_list:
- description: ''
  name: EgressType
  type: object
- description: ''
  name: VpcConnectorArn
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-egressconfiguration-schema.json
slug: amazon-app-runner-egressconfiguration
source_filename: amazon-app-runner-egressconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"EgressConfiguration\",\n  \"description\": \"Describes configuration settings related to outbound network traffic of an App Runner service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EgressType\": {},\n    \"VpcConnectorArn\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-egressconfiguration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: EgressConfiguration
---
