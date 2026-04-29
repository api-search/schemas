---
description: Current state of the project.
layout: schema
name: ProjectStatus
properties_list:
- description: The lifecycle phase of the project.
  name: phase
  type: string
- description: ''
  name: conditions
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-project-status-schema.json
slug: openshift-rest-project-status
source_filename: openshift-rest-project-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProjectStatus\",\n  \"type\": \"object\",\n  \"description\": \"Current state of the project.\",\n  \"properties\": {\n    \"phase\": {\n      \"type\": \"string\",\n      \"description\": \"The lifecycle phase of the project.\"\n    },\n    \"conditions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-project-status-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: ProjectStatus
---
