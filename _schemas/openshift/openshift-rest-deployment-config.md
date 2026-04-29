---
description: A DeploymentConfig describes the desired state of a particular application deployment. It creates ReplicationControllers to manage pods and supports rolling, recreate, and custom deployment strategies with automatic rollback.
layout: schema
name: DeploymentConfig
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-deployment-config-schema.json
slug: openshift-rest-deployment-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeploymentConfig\",\n  \"type\": \"object\",\n  \"description\": \"A DeploymentConfig describes the desired state of a particular application deployment. It creates ReplicationControllers to manage pods and supports rolling, recreate, and custom deployment strategies with automatic rollback.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-deployment-config-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: DeploymentConfig
---
