---
description: Status of the DeploymentConfig.
layout: schema
name: DeploymentConfigStatus
properties_list:
- description: The version of the most recent deployment.
  name: latestVersion
  type: integer
- description: The most recent generation observed by the deployment controller.
  name: observedGeneration
  type: integer
- description: Total number of non-terminated pods targeted by this deployment.
  name: replicas
  type: integer
- description: Total number of non-terminated pods that have the desired template spec.
  name: updatedReplicas
  type: integer
- description: Total number of available pods targeted by this deployment.
  name: availableReplicas
  type: integer
- description: Total number of unavailable pods targeted by this deployment.
  name: unavailableReplicas
  type: integer
- description: Total number of ready pods targeted by this deployment.
  name: readyReplicas
  type: integer
- description: ''
  name: conditions
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-deployment-config-status-schema.json
slug: openshift-rest-deployment-config-status
source_filename: openshift-rest-deployment-config-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentConfigStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status of the DeploymentConfig.\",\n  \"properties\": {\n    \"latestVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"The version of the most recent deployment.\"\n    },\n    \"observedGeneration\": {\n      \"type\": \"integer\",\n      \"description\": \"The most recent generation observed by the deployment controller.\"\n    },\n    \"replicas\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of non-terminated pods targeted by this deployment.\"\n    },\n    \"updatedReplicas\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of non-terminated pods that have the desired template spec.\"\n    },\n    \"availableReplicas\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of available pods targeted by this deployment.\"\n    },\n\
  \    \"unavailableReplicas\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of unavailable pods targeted by this deployment.\"\n    },\n    \"readyReplicas\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of ready pods targeted by this deployment.\"\n    },\n    \"conditions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-deployment-config-status-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DeploymentConfigStatus
---
