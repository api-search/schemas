---
description: A policy that triggers new deployments.
layout: schema
name: DeploymentTriggerPolicy
properties_list:
- description: The type of deployment trigger.
  name: type
  type: string
- description: Parameters for an ImageChange trigger.
  name: imageChangeParams
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-deployment-trigger-policy-schema.json
slug: openshift-rest-deployment-trigger-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentTriggerPolicy\",\n  \"type\": \"object\",\n  \"description\": \"A policy that triggers new deployments.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of deployment trigger.\"\n    },\n    \"imageChangeParams\": {\n      \"type\": \"object\",\n      \"description\": \"Parameters for an ImageChange trigger.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-deployment-trigger-policy-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DeploymentTriggerPolicy
---
