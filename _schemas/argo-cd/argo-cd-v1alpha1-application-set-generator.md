---
description: ApplicationSetGenerator represents a generator at the top level of an ApplicationSet.
layout: schema
name: v1alpha1ApplicationSetGenerator
properties_list:
- description: ''
  name: clusterDecisionResource
  type: object
- description: ''
  name: clusters
  type: object
- description: ''
  name: git
  type: object
- description: ''
  name: list
  type: object
- description: ''
  name: matrix
  type: object
- description: ''
  name: merge
  type: object
- description: ''
  name: plugin
  type: object
- description: ''
  name: pullRequest
  type: object
- description: ''
  name: scmProvider
  type: object
- description: ''
  name: selector
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-application-set-generator-schema.json
slug: argo-cd-v1alpha1-application-set-generator
source_filename: argo-cd-v1alpha1-application-set-generator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-generator-schema.json\",\n  \"title\": \"v1alpha1ApplicationSetGenerator\",\n  \"description\": \"ApplicationSetGenerator represents a generator at the top level of an ApplicationSet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clusterDecisionResource\": {\n      \"$ref\": \"#/definitions/v1alpha1DuckTypeGenerator\"\n    },\n    \"clusters\": {\n      \"$ref\": \"#/definitions/v1alpha1ClusterGenerator\"\n    },\n    \"git\": {\n      \"$ref\": \"#/definitions/v1alpha1GitGenerator\"\n    },\n    \"list\": {\n      \"$ref\": \"#/definitions/v1alpha1ListGenerator\"\n    },\n    \"matrix\": {\n      \"$ref\": \"#/definitions/v1alpha1MatrixGenerator\"\n    },\n    \"merge\": {\n      \"$ref\": \"#/definitions/v1alpha1MergeGenerator\"\n    },\n    \"plugin\": {\n      \"\
  $ref\": \"#/definitions/v1alpha1PluginGenerator\"\n    },\n    \"pullRequest\": {\n      \"$ref\": \"#/definitions/v1alpha1PullRequestGenerator\"\n    },\n    \"scmProvider\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGenerator\"\n    },\n    \"selector\": {\n      \"$ref\": \"#/definitions/v1LabelSelector\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-application-set-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1ApplicationSetGenerator
---
