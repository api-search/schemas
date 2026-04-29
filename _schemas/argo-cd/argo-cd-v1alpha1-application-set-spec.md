---
description: ApplicationSetSpec represents a class of application set state.
layout: schema
name: v1alpha1ApplicationSetSpec
properties_list:
- description: 'ApplyNestedSelectors enables selectors defined within the generators of two level-nested matrix or merge generators. Deprecated: This field is ignored, and the behavior is always enabled. The field wi'
  name: applyNestedSelectors
  type: boolean
- description: ''
  name: generators
  type: array
- description: ''
  name: goTemplate
  type: boolean
- description: ''
  name: goTemplateOptions
  type: array
- description: ''
  name: ignoreApplicationDifferences
  type: array
- description: ''
  name: preservedFields
  type: object
- description: ''
  name: strategy
  type: object
- description: ''
  name: syncPolicy
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: templatePatch
  type: string
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-spec-schema.json
slug: argo-cd-v1alpha1-application-set-spec
source_filename: argo-cd-v1alpha1-application-set-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-spec-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetSpec\",\n  \"description\": \"ApplicationSetSpec represents a class of application set state.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applyNestedSelectors\": {\n      \"description\": \"ApplyNestedSelectors enables selectors defined within the generators of two level-nested matrix or merge generators.\\n\\nDeprecated: This field is ignored, and the behavior is always enabled. The field will be removed in a future\\nversion of the ApplicationSet CRD.\",\n      \"type\": \"boolean\"\n    },\n    \"generators\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSetGenerator\"\n      }\n    },\n    \"goTemplate\": {\n      \"type\": \"boolean\"\n    },\n \
  \   \"goTemplateOptions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"ignoreApplicationDifferences\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSetResourceIgnoreDifferences\"\n      }\n    },\n    \"preservedFields\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationPreservedFields\"\n    },\n    \"strategy\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetStrategy\"\n    },\n    \"syncPolicy\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetSyncPolicy\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    },\n    \"templatePatch\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-spec-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetSpec
---
