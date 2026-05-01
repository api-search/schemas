---
description: Describes the observability configuration of an App Runner service. These are additional observability features, like tracing, that you choose to enable. They're configured in a separate resource that you associate with your service.
layout: schema
name: ServiceObservabilityConfiguration
properties_list:
- description: ''
  name: ObservabilityEnabled
  type: object
- description: ''
  name: ObservabilityConfigurationArn
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-serviceobservabilityconfiguration-schema.json
slug: amazon-app-runner-serviceobservabilityconfiguration
source_filename: amazon-app-runner-serviceobservabilityconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ServiceObservabilityConfiguration\",\n  \"description\": \"Describes the observability configuration of an App Runner service. These are additional observability features, like tracing, that you choose to enable. They're configured in a separate resource that you associate with your service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObservabilityEnabled\": {},\n    \"ObservabilityConfigurationArn\": {}\n  },\n  \"required\": [\n    \"ObservabilityEnabled\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-serviceobservabilityconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: ServiceObservabilityConfiguration
---
