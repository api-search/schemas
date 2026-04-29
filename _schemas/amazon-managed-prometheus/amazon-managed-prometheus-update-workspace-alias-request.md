---
description: Represents the input of an UpdateWorkspaceAlias operation.
layout: schema
name: UpdateWorkspaceAliasRequest
properties_list:
- description: ''
  name: alias
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-update-workspace-alias-request-schema.json
slug: amazon-managed-prometheus-update-workspace-alias-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-update-workspace-alias-request-schema.json\",\n  \"title\": \"UpdateWorkspaceAliasRequest\",\n  \"description\": \"Represents the input of an UpdateWorkspaceAlias operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceAlias\"\n        },\n        {\n          \"description\": \"The new alias of the workspace.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"Optional, unique, case-sensitive, user-provided identifier to ensure the idempotency of the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-update-workspace-alias-request-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: UpdateWorkspaceAliasRequest
---
