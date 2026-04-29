---
description: PullRequestGenerator defines a generator that scrapes a PullRequest API to find candidate pull requests.
layout: schema
name: v1alpha1PullRequestGenerator
properties_list:
- description: ''
  name: azuredevops
  type: object
- description: ''
  name: bitbucket
  type: object
- description: ''
  name: bitbucketServer
  type: object
- description: ContinueOnRepoNotFoundError is a flag to continue the ApplicationSet Pull Request generator parameters generation even if the repository is not found.
  name: continueOnRepoNotFoundError
  type: boolean
- description: Filters for which pull requests should be considered.
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
schema_file: json-schema/argo-cd-v1alpha1-pull-request-generator-schema.json
slug: argo-cd-v1alpha1-pull-request-generator
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-schema.json\",\n  \"title\": \"v1alpha1PullRequestGenerator\",\n  \"description\": \"PullRequestGenerator defines a generator that scrapes a PullRequest API to find candidate pull requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"azuredevops\": {\n      \"$ref\": \"#/definitions/v1alpha1PullRequestGeneratorAzureDevOps\"\n    },\n    \"bitbucket\": {\n      \"$ref\": \"#/definitions/v1alpha1PullRequestGeneratorBitbucket\"\n    },\n    \"bitbucketServer\": {\n      \"$ref\": \"#/definitions/v1alpha1PullRequestGeneratorBitbucketServer\"\n    },\n    \"continueOnRepoNotFoundError\": {\n      \"description\": \"ContinueOnRepoNotFoundError is a flag to continue the ApplicationSet Pull Request generator parameters generation even if the repository is not found.\"\
  ,\n      \"type\": \"boolean\"\n    },\n    \"filters\": {\n      \"description\": \"Filters for which pull requests should be considered.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/definitions/v1alpha1PullRequestGeneratorFilter\"\n      }\n    },\n    \"gitea\": {\n      \"$ref\": \"#/definitions/v1alpha1PullRequestGeneratorGitea\"\n    },\n    \"github\": {\n      \"$ref\": \"#/definitions/v1alpha1PullRequestGeneratorGithub\"\n    },\n    \"gitlab\": {\n      \"$ref\": \"#/definitions/v1alpha1PullRequestGeneratorGitLab\"\n    },\n    \"requeueAfterSeconds\": {\n      \"description\": \"Standard parameters.\",\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"template\": {\n      \"$ref\": \"#/definitions/v1alpha1ApplicationSetTemplate\"\n    },\n    \"values\": {\n      \"type\": \"object\",\n      \"title\": \"Values contains key/value pairs which are passed directly as parameters to the template\",\n      \"additionalProperties\"\
  : {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/json-schema/argo-cd-v1alpha1-pull-request-generator-schema.json
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open Source
title: v1alpha1PullRequestGenerator
---
