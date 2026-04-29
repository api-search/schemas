---
description: A Project provides a scope for Kubernetes resources, extending namespaces with additional metadata and access controls for multi-tenant environments.
layout: schema
name: Project
properties_list:
- description: ''
  name: apiVersion
  type: string
- description: ''
  name: kind
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-project-schema.json
slug: openshift-rest-project
source_filename: openshift-rest-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"description\": \"A Project provides a scope for Kubernetes resources, extending namespaces with additional metadata and access controls for multi-tenant environments.\",\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\"\n    },\n    \"kind\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-project-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: Project
---
