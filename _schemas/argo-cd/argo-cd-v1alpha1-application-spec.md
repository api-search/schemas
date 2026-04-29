---
description: ApplicationSpec represents desired application state. Contains link to repository with application definition and additional parameters link definition revision.
layout: schema
name: v1alpha1ApplicationSpec
properties_list:
- description: ''
  name: destination
  type: object
- description: ''
  name: ignoreDifferences
  type: array
- description: ''
  name: info
  type: array
- description: Project is a reference to the project this application belongs to. The empty string means that application belongs to the 'default' project.
  name: project
  type: string
- description: 'RevisionHistoryLimit limits the number of items kept in the application''s revision history, which is used for informational purposes as well as for rollbacks to previous versions. This should only be '
  name: revisionHistoryLimit
  type: integer
- description: ''
  name: source
  type: object
- description: ''
  name: sourceHydrator
  type: object
- description: ''
  name: sources
  type: array
- description: ''
  name: syncPolicy
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-spec-schema.json
slug: argo-cd-v1alpha1-application-spec
source_filename: argo-cd-v1alpha1-application-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-spec-schema.json\",\n  \"title\": \"v1alpha1ApplicationSpec\",\n  \"description\": \"ApplicationSpec represents desired application state. Contains link to repository with application definition and additional parameters link definition revision.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"destination\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationDestination\"\n    },\n    \"ignoreDifferences\": {\n      \"type\": \"array\",\n      \"title\": \"IgnoreDifferences is a list of resources and their fields which should be ignored during comparison\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ResourceIgnoreDifferences\"\n      }\n    },\n    \"info\": {\n      \"type\": \"array\",\n      \"title\": \"Info contains a list of information (URLs, email\
  \ addresses, and plain text) that relates to the application\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1Info\"\n      }\n    },\n    \"project\": {\n      \"description\": \"Project is a reference to the project this application belongs to.\\nThe empty string means that application belongs to the 'default' project.\",\n      \"type\": \"string\"\n    },\n    \"revisionHistoryLimit\": {\n      \"description\": \"RevisionHistoryLimit limits the number of items kept in the application's revision history, which is used for informational purposes as well as for rollbacks to previous versions.\\nThis should only be changed in exceptional circumstances.\\nSetting to zero will store no history. This will reduce storage used.\\nIncreasing will increase the space used to store the history, so we do not recommend increasing it.\\nDefault is 10.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"source\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\
  \n    },\n    \"sourceHydrator\": {\n      \"$ref\": \"#/definitions/v1alpha1SourceHydrator\"\n    },\n    \"sources\": {\n      \"type\": \"array\",\n      \"title\": \"Sources is a reference to the location of the application's manifests or chart\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1ApplicationSource\"\n      }\n    },\n    \"syncPolicy\": {\n      \"$ref\": \"#/definitions/v1alpha1SyncPolicy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-spec-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSpec
---
