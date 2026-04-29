---
description: A request to roll back a deployment to a previous version.
layout: schema
name: DeploymentConfigRollback
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: Name of the deployment config to roll back.
  name: name
  type: string
- description: ''
  name: spec
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-deployment-config-rollback-schema.json
slug: openshift-rest-deployment-config-rollback
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentConfigRollback\",\n  \"type\": \"object\",\n  \"description\": \"A request to roll back a deployment to a previous version.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the deployment config to roll back.\"\n    },\n    \"spec\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-deployment-config-rollback-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DeploymentConfigRollback
---
