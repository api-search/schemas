---
description: A policy that causes a new build to be created.
layout: schema
name: BuildTriggerPolicy
properties_list:
- description: The type of build trigger.
  name: type
  type: string
- description: ''
  name: github
  type: object
- description: ''
  name: generic
  type: object
- description: ''
  name: imageChange
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-trigger-policy-schema.json
slug: openshift-rest-build-trigger-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildTriggerPolicy\",\n  \"type\": \"object\",\n  \"description\": \"A policy that causes a new build to be created.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of build trigger.\"\n    },\n    \"github\": {\n      \"type\": \"object\"\n    },\n    \"generic\": {\n      \"type\": \"object\"\n    },\n    \"imageChange\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-trigger-policy-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildTriggerPolicy
---
