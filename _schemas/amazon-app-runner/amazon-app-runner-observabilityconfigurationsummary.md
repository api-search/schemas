---
description: <p>Provides summary information about an App Runner observability configuration resource.</p> <p>This type contains limited information about an observability configuration. It includes only identification information, without configuration details. It's returned by the <a>ListObservabilityConfigurations</a> action. Complete configuration information is returned by the <a>CreateObservabilityConfiguration</a>, <a>DescribeObservabilityConfiguration</a>, and <a>DeleteObservabilityConfiguration</a> actions using the <a>ObservabilityConfiguration</a> type.</p>
layout: schema
name: ObservabilityConfigurationSummary
properties_list:
- description: ''
  name: ObservabilityConfigurationArn
  type: object
- description: ''
  name: ObservabilityConfigurationName
  type: object
- description: ''
  name: ObservabilityConfigurationRevision
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-observabilityconfigurationsummary-schema.json
slug: amazon-app-runner-observabilityconfigurationsummary
source_filename: amazon-app-runner-observabilityconfigurationsummary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"ObservabilityConfigurationSummary\",\n  \"description\": \"<p>Provides summary information about an App Runner observability configuration resource.</p> <p>This type contains limited information about an observability configuration. It includes only identification information, without configuration details. It's returned by the <a>ListObservabilityConfigurations</a> action. Complete configuration information is returned by the <a>CreateObservabilityConfiguration</a>, <a>DescribeObservabilityConfiguration</a>, and <a>DeleteObservabilityConfiguration</a> actions using the <a>ObservabilityConfiguration</a> type.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObservabilityConfigurationArn\": {},\n    \"ObservabilityConfigurationName\": {},\n    \"ObservabilityConfigurationRevision\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-observabilityconfigurationsummary-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: ObservabilityConfigurationSummary
---
