---
description: Describes the state of a deployment at a point in time.
layout: schema
name: DeploymentCondition
properties_list:
- description: The type of condition.
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: reason
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: lastUpdateTime
  type: string
- description: ''
  name: lastTransitionTime
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-deployment-condition-schema.json
slug: openshift-rest-deployment-condition
source_filename: openshift-rest-deployment-condition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentCondition\",\n  \"type\": \"object\",\n  \"description\": \"Describes the state of a deployment at a point in time.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of condition.\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"reason\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateTime\": {\n      \"type\": \"string\"\n    },\n    \"lastTransitionTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-deployment-condition-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DeploymentCondition
---
