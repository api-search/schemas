---
description: ApplicationSetStrategy configures how generated Applications are updated in sequence.
layout: schema
name: v1alpha1ApplicationSetStrategy
properties_list:
- description: ''
  name: deletionOrder
  type: string
- description: ''
  name: rollingSync
  type: object
- description: ''
  name: type
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-strategy-schema.json
slug: argo-cd-v1alpha1-application-set-strategy
source_filename: argo-cd-v1alpha1-application-set-strategy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-strategy-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetStrategy\",\n  \"description\": \"ApplicationSetStrategy configures how generated Applications are updated in sequence.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deletionOrder\": {\n      \"type\": \"string\",\n      \"title\": \"DeletionOrder allows specifying the order for deleting generated apps when progressive sync is enabled.\\naccepts values \\\"AllAtOnce\\\" and \\\"Reverse\\\"\"\n    },\n    \"rollingSync\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetRolloutStrategy\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-strategy-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetStrategy
---
