---
description: <p>Describes an App Runner automatic scaling configuration resource.</p> <p>A higher <code>MinSize</code> increases the spread of your App Runner service over more Availability Zones in the Amazon Web Services Region. The tradeoff is a higher minimal cost.</p> <p>A lower <code>MaxSize</code> controls your cost. The tradeoff is lower responsiveness during peak demand.</p> <p>Multiple revisions of a configuration might have the same <code>AutoScalingConfigurationName</code> and different <code>AutoScalingConfigurationRevision</code> values.</p>
layout: schema
name: AutoScalingConfiguration
properties_list:
- description: ''
  name: AutoScalingConfigurationArn
  type: object
- description: ''
  name: AutoScalingConfigurationName
  type: object
- description: ''
  name: AutoScalingConfigurationRevision
  type: object
- description: ''
  name: Latest
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: MaxConcurrency
  type: object
- description: ''
  name: MinSize
  type: object
- description: ''
  name: MaxSize
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: DeletedAt
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-autoscalingconfiguration-schema.json
slug: amazon-app-runner-autoscalingconfiguration
source_filename: amazon-app-runner-autoscalingconfiguration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AutoScalingConfiguration\",\n  \"description\": \"<p>Describes an App Runner automatic scaling configuration resource.</p> <p>A higher <code>MinSize</code> increases the spread of your App Runner service over more Availability Zones in the Amazon Web Services Region. The tradeoff is a higher minimal cost.</p> <p>A lower <code>MaxSize</code> controls your cost. The tradeoff is lower responsiveness during peak demand.</p> <p>Multiple revisions of a configuration might have the same <code>AutoScalingConfigurationName</code> and different <code>AutoScalingConfigurationRevision</code> values.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutoScalingConfigurationArn\": {},\n    \"AutoScalingConfigurationName\": {},\n    \"AutoScalingConfigurationRevision\": {},\n    \"Latest\": {},\n    \"Status\": {},\n    \"MaxConcurrency\": {},\n    \"MinSize\": {},\n    \"MaxSize\": {},\n    \"CreatedAt\"\
  : {},\n    \"DeletedAt\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-autoscalingconfiguration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: AutoScalingConfiguration
---
