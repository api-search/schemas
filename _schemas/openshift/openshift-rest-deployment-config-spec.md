---
description: Specification for the desired deployment behavior.
layout: schema
name: DeploymentConfigSpec
properties_list:
- description: The desired number of pod replicas.
  name: replicas
  type: integer
- description: Label selector for pods managed by this deployment.
  name: selector
  type: object
- description: Triggers that cause new deployments to be created.
  name: triggers
  type: array
- description: Minimum number of seconds a newly created pod should be ready without any of its containers crashing before considered available.
  name: minReadySeconds
  type: integer
- description: Number of old ReplicationControllers to retain for rollback.
  name: revisionHistoryLimit
  type: integer
- description: Indicates that the deployment config is paused and new deployments will not be triggered.
  name: paused
  type: boolean
- description: If true, deployments are scaled down to zero after the deployment completes.
  name: test
  type: boolean
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-deployment-config-spec-schema.json
slug: openshift-rest-deployment-config-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentConfigSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for the desired deployment behavior.\",\n  \"properties\": {\n    \"replicas\": {\n      \"type\": \"integer\",\n      \"description\": \"The desired number of pod replicas.\"\n    },\n    \"selector\": {\n      \"type\": \"object\",\n      \"description\": \"Label selector for pods managed by this deployment.\"\n    },\n    \"triggers\": {\n      \"type\": \"array\",\n      \"description\": \"Triggers that cause new deployments to be created.\"\n    },\n    \"minReadySeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of seconds a newly created pod should be ready without any of its containers crashing before considered available.\"\n    },\n    \"revisionHistoryLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of old ReplicationControllers to retain for\
  \ rollback.\"\n    },\n    \"paused\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates that the deployment config is paused and new deployments will not be triggered.\"\n    },\n    \"test\": {\n      \"type\": \"boolean\",\n      \"description\": \"If true, deployments are scaled down to zero after the deployment completes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-deployment-config-spec-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DeploymentConfigSpec
---
