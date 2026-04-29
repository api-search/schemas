---
description: Parameters for a rolling deployment strategy.
layout: schema
name: RollingDeploymentStrategyParams
properties_list:
- description: The time to wait between individual pod updates.
  name: updatePeriodSeconds
  type: integer
- description: The time to wait between polling deployment status.
  name: intervalSeconds
  type: integer
- description: The time to wait for a scaling event before giving up.
  name: timeoutSeconds
  type: integer
- description: The maximum number of pods that can be unavailable during the update. Value can be an absolute number or a percentage.
  name: maxUnavailable
  type: string
- description: The maximum number of pods that can be scheduled above the desired number of pods. Value can be an absolute number or a percentage.
  name: maxSurge
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-rolling-deployment-strategy-params-schema.json
slug: openshift-rest-rolling-deployment-strategy-params
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RollingDeploymentStrategyParams\",\n  \"type\": \"object\",\n  \"description\": \"Parameters for a rolling deployment strategy.\",\n  \"properties\": {\n    \"updatePeriodSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The time to wait between individual pod updates.\"\n    },\n    \"intervalSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The time to wait between polling deployment status.\"\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"The time to wait for a scaling event before giving up.\"\n    },\n    \"maxUnavailable\": {\n      \"type\": \"string\",\n      \"description\": \"The maximum number of pods that can be unavailable during the update. Value can be an absolute number or a percentage.\"\n    },\n    \"maxSurge\": {\n      \"type\": \"string\",\n      \"description\": \"The maximum number of pods\
  \ that can be scheduled above the desired number of pods. Value can be an absolute number or a percentage.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-rolling-deployment-strategy-params-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: RollingDeploymentStrategyParams
---
