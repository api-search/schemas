---
description: A request to create a new project. ProjectRequests are processed according to the cluster project request template and may include default resource quotas, limit ranges, and role bindings.
layout: schema
name: ProjectRequest
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
- description: A human-readable name for the project, used in the web console.
  name: displayName
  type: string
- description: A longer description of the project purpose.
  name: description
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-project-request-schema.json
slug: openshift-rest-project-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProjectRequest\",\n  \"type\": \"object\",\n  \"description\": \"A request to create a new project. ProjectRequests are processed according to the cluster project request template and may include default resource quotas, limit ranges, and role bindings.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the project, used in the web console.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A longer description of the project purpose.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-project-request-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: ProjectRequest
---
