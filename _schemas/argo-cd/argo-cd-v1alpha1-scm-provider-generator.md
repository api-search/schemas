---
description: SCMProviderGenerator defines a generator that scrapes a SCMaaS API to find candidate repos.
layout: schema
name: v1alpha1SCMProviderGenerator
properties_list:
- description: ''
  name: awsCodeCommit
  type: object
- description: ''
  name: azureDevOps
  type: object
- description: ''
  name: bitbucket
  type: object
- description: ''
  name: bitbucketServer
  type: object
- description: Which protocol to use for the SCM URL. Default is provider-specific but ssh if possible. Not all providers necessarily support all protocols.
  name: cloneProtocol
  type: string
- description: Filters for which repos should be considered.
  name: filters
  type: array
- description: ''
  name: gitea
  type: object
- description: ''
  name: github
  type: object
- description: ''
  name: gitlab
  type: object
- description: Standard parameters.
  name: requeueAfterSeconds
  type: integer
- description: ''
  name: template
  type: object
- description: ''
  name: values
  type: object
provider_name: Argo CD
provider_slug: argo-cd
schema_file: json-schema/argo-cd-v1alpha1-scm-provider-generator-schema.json
slug: argo-cd-v1alpha1-scm-provider-generator
source_filename: argo-cd-v1alpha1-scm-provider-generator-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-schema.json\",\n  \"title\": \"v1alpha1SCMProviderGenerator\",\n  \"description\": \"SCMProviderGenerator defines a generator that scrapes a SCMaaS API to find candidate repos.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"awsCodeCommit\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorAWSCodeCommit\"\n    },\n    \"azureDevOps\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorAzureDevOps\"\n    },\n    \"bitbucket\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorBitbucket\"\n    },\n    \"bitbucketServer\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorBitbucketServer\"\n    },\n    \"cloneProtocol\": {\n      \"description\": \"Which protocol to use for the SCM URL. Default is provider-specific\
  \ but ssh if possible. Not all providers\\nnecessarily support all protocols.\",\n      \"type\": \"string\"\n    },\n    \"filters\": {\n      \"description\": \"Filters for which repos should be considered.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorFilter\"\n      }\n    },\n    \"gitea\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorGitea\"\n    },\n    \"github\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorGithub\"\n    },\n    \"gitlab\": {\n      \"$ref\": \"#/definitions/v1alpha1SCMProviderGeneratorGitlab\"\n    },\n    \"requeueAfterSeconds\": {\n      \"description\": \"Standard parameters.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"title\": \"Values contains key/value pairs which are passed directly\
  \ as parameters to the template\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-scm-provider-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1SCMProviderGenerator
---
