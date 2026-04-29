---
description: Parameters for a recreate deployment strategy.
layout: schema
name: RecreateDeploymentStrategyParams
properties_list:
- description: The time to wait for pods to terminate before giving up.
  name: timeoutSeconds
  type: integer
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-recreate-deployment-strategy-params-schema.json
slug: openshift-rest-recreate-deployment-strategy-params
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecreateDeploymentStrategyParams\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for a recreate deployment strategy.\",\n  \"properties\": {\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The time to wait for pods to terminate before giving up.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-recreate-deployment-strategy-params-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: RecreateDeploymentStrategyParams
---
