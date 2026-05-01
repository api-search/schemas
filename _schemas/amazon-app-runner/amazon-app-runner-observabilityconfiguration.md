---
description: <p>Describes an App Runner observability configuration resource. Multiple revisions of a configuration have the same <code>ObservabilityConfigurationName</code> and different <code>ObservabilityConfigurationRevision</code> values.</p> <p>The resource is designed to configure multiple features (currently one feature, tracing). This type contains optional members that describe the configuration of these features (currently one member, <code>TraceConfiguration</code>). If a feature member isn't specified, the feature isn't enabled.</p>
layout: schema
name: ObservabilityConfiguration
properties_list:
- description: ''
  name: ObservabilityConfigurationArn
  type: object
- description: ''
  name: ObservabilityConfigurationName
  type: object
- description: ''
  name: TraceConfiguration
  type: object
- description: ''
  name: ObservabilityConfigurationRevision
  type: object
- description: ''
  name: Latest
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: DeletedAt
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-observabilityconfiguration-schema.json
slug: amazon-app-runner-observabilityconfiguration
source_filename: amazon-app-runner-observabilityconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ObservabilityConfiguration\",\n  \"description\": \"<p>Describes an App Runner observability configuration resource. Multiple revisions of a configuration have the same <code>ObservabilityConfigurationName</code> and different <code>ObservabilityConfigurationRevision</code> values.</p> <p>The resource is designed to configure multiple features (currently one feature, tracing). This type contains optional members that describe the configuration of these features (currently one member, <code>TraceConfiguration</code>). If a feature member isn't specified, the feature isn't enabled.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObservabilityConfigurationArn\": {},\n    \"ObservabilityConfigurationName\": {},\n    \"TraceConfiguration\": {},\n    \"ObservabilityConfigurationRevision\": {},\n    \"Latest\": {},\n    \"Status\": {},\n    \"CreatedAt\": {},\n    \"DeletedAt\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-observabilityconfiguration-schema.json
tags:
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: ObservabilityConfiguration
---
