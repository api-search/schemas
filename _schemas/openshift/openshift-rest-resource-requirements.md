---
description: Compute resource requirements for a container.
layout: schema
name: ResourceRequirements
properties_list:
- description: Maximum compute resources allowed (e.g., cpu, memory).
  name: limits
  type: object
- description: Minimum compute resources required (e.g., cpu, memory).
  name: requests
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-resource-requirements-schema.json
slug: openshift-rest-resource-requirements
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourceRequirements\",\n  \"type\": \"object\",\n  \"description\": \"Compute resource requirements for a container.\",\n  \"properties\": {\n    \"limits\": {\n      \"type\": \"object\",\n      \"description\": \"Maximum compute resources allowed (e.g., cpu, memory).\"\n    },\n    \"requests\": {\n      \"type\": \"object\",\n      \"description\": \"Minimum compute resources required (e.g., cpu, memory).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-resource-requirements-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: ResourceRequirements
---
