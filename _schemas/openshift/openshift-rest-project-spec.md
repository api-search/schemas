---
description: Specification for the desired project state.
layout: schema
name: ProjectSpec
properties_list:
- description: Finalizers that must complete before the project is deleted.
  name: finalizers
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-project-spec-schema.json
slug: openshift-rest-project-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProjectSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for the desired project state.\",\n  \"properties\": {\n    \"finalizers\": {\n      \"type\": \"array\",\n      \"description\": \"Finalizers that must complete before the project is deleted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-project-spec-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: ProjectSpec
---
