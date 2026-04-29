---
description: v1alpha1RevisionHistory schema from Argo CD API
layout: schema
name: v1alpha1RevisionHistory
properties_list:
- description: ''
  name: deployStartedAt
  type: object
- description: ''
  name: deployedAt
  type: object
- description: ''
  name: id
  type: integer
- description: ''
  name: initiatedBy
  type: object
- description: ''
  name: revision
  type: string
- description: ''
  name: revisions
  type: array
- description: ''
  name: source
  type: object
- description: ''
  name: sources
  type: array
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-revision-history-schema.json
slug: argo-cd-v1alpha1-revision-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-revision-history-schema.json\",\n  \"title\": \"v1alpha1RevisionHistory\",\n  \"description\": \"v1alpha1RevisionHistory schema from Argo CD API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deployStartedAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"deployedAt\": {\n      \"$ref\": \"#/definitions/v1Time\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"title\": \"ID is an auto incrementing identifier of the RevisionHistory\"\n    },\n    \"initiatedBy\": {\n      \"$ref\": \"#/definitions/v1alpha1OperationInitiator\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"title\": \"Revision holds the revision the sync was performed against\"\n    },\n    \"revisions\": {\n      \"type\": \"array\",\n      \"\
  title\": \"Revisions holds the revision of each source in sources field the sync was performed against\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"title\": \"Sources is a reference to the application sources used for the sync operation\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-revision-history-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1RevisionHistory
---
