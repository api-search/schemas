---
description: ResourceAction represents an individual action that can be performed on a resource. It includes parameters, an optional disabled flag, an icon for display, and a name for the action.
layout: schema
name: v1alpha1ResourceAction
properties_list:
- description: Disabled indicates whether the action is disabled.
  name: disabled
  type: boolean
- description: DisplayName provides a user-friendly name for the action.
  name: displayName
  type: string
- description: IconClass specifies the CSS class for the action's icon.
  name: iconClass
  type: string
- description: Name is the name or identifier for the action.
  name: name
  type: string
- description: Params contains the parameters required to execute the action.
  name: params
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-resource-action-schema.json
slug: argo-cd-v1alpha1-resource-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-action-schema.json\",\n  \"title\": \"v1alpha1ResourceAction\",\n  \"description\": \"ResourceAction represents an individual action that can be performed on a resource.\\nIt includes parameters, an optional disabled flag, an icon for display, and a name for the action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"disabled\": {\n      \"description\": \"Disabled indicates whether the action is disabled.\",\n      \"type\": \"boolean\"\n    },\n    \"displayName\": {\n      \"description\": \"DisplayName provides a user-friendly name for the action.\",\n      \"type\": \"string\"\n    },\n    \"iconClass\": {\n      \"description\": \"IconClass specifies the CSS class for the action's icon.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Name\
  \ is the name or identifier for the action.\",\n      \"type\": \"string\"\n    },\n    \"params\": {\n      \"description\": \"Params contains the parameters required to execute the action.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceActionParam\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-resource-action-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ResourceAction
---
