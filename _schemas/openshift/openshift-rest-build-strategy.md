---
description: Describes how to perform the build.
layout: schema
name: BuildStrategy
properties_list:
- description: The type of build strategy.
  name: type
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-strategy-schema.json
slug: openshift-rest-build-strategy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildStrategy\",\n  \"type\": \"object\",\n  \"description\": \"Describes how to perform the build.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of build strategy.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-strategy-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildStrategy
---
