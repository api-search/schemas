---
description: Argo CD server configuration settings.
layout: schema
name: Settings
properties_list:
- description: External URL of the Argo CD server.
  name: url
  type: string
- description: Dex OAuth provider configuration YAML.
  name: dexConfig
  type: string
- description: OIDC provider configuration YAML.
  name: oidcConfig
  type: string
- description: Whether application status badges are enabled.
  name: statusBadgeEnabled
  type: boolean
- description: Google Analytics tracking configuration.
  name: googleAnalytics
  type: object
- description: Help link configuration.
  name: help
  type: object
provider_name: Argo
provider_slug: argo
schema_file: json-schema/argo-cd-settings-schema.json
slug: argo-cd-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-settings-schema.json\",\n  \"title\": \"Settings\",\n  \"description\": \"Argo CD server configuration settings.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"External URL of the Argo CD server.\",\n      \"format\": \"uri\"\n    },\n    \"dexConfig\": {\n      \"type\": \"string\",\n      \"description\": \"Dex OAuth provider configuration YAML.\"\n    },\n    \"oidcConfig\": {\n      \"type\": \"string\",\n      \"description\": \"OIDC provider configuration YAML.\"\n    },\n    \"statusBadgeEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether application status badges are enabled.\"\n    },\n    \"googleAnalytics\": {\n      \"type\": \"object\",\n      \"description\": \"Google Analytics tracking configuration.\"\
  ,\n      \"properties\": {\n        \"trackingID\": {\n          \"type\": \"string\",\n          \"description\": \"Google Analytics tracking ID.\"\n        },\n        \"anonymizeUsers\": {\n          \"type\": \"boolean\",\n          \"description\": \"Anonymize user tracking data.\"\n        }\n      }\n    },\n    \"help\": {\n      \"type\": \"object\",\n      \"description\": \"Help link configuration.\",\n      \"properties\": {\n        \"chatUrl\": {\n          \"type\": \"string\",\n          \"description\": \"URL for community chat (e.g., Slack).\"\n        },\n        \"chatText\": {\n          \"type\": \"string\",\n          \"description\": \"Display text for the chat link.\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo/refs/heads/main/json-schema/argo-cd-settings-schema.json
tags:
- CNCF
- CI/CD
- GitOps
- Kubernetes
- Open Source
- Progressive Delivery
- Workflow Engine
title: Settings
---
