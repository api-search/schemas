---
description: Describes resources needed to authenticate access to some source repositories. The specific resource depends on the repository provider.
layout: schema
name: AuthenticationConfiguration
properties_list:
- description: ''
  name: ConnectionArn
  type: object
- description: ''
  name: AccessRoleArn
  type: object
provider_name: Amazon App Runner
provider_slug: amazon-app-runner
schema_file: json-schema/amazon-app-runner-authenticationconfiguration-schema.json
slug: amazon-app-runner-authenticationconfiguration
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AuthenticationConfiguration\",\n  \"description\": \"Describes resources needed to authenticate access to some source repositories. The specific resource depends on the repository provider.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConnectionArn\": {},\n    \"AccessRoleArn\": {}\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-runner/refs/heads/main/json-schema/amazon-app-runner-authenticationconfiguration-schema.json
tags:
- AWS
- CI/CD
- Containers
- Deployment
- Managed Service
- Serverless
- Web Applications
title: AuthenticationConfiguration
---
