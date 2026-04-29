---
description: Describes how to perform a deployment.
layout: schema
name: DeploymentStrategy
properties_list:
- description: The deployment strategy type.
  name: type
  type: string
- description: Duration in seconds that the deployer pods may be active before the system retries the deployment.
  name: activeDeadlineSeconds
  type: integer
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-deployment-strategy-schema.json
slug: openshift-rest-deployment-strategy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentStrategy\",\n  \"type\": \"object\",\n  \"description\": \"Describes how to perform a deployment.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The deployment strategy type.\"\n    },\n    \"activeDeadlineSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration in seconds that the deployer pods may be active before the system retries the deployment.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-deployment-strategy-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DeploymentStrategy
---
