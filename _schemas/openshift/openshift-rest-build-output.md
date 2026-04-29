---
description: Specifies where the resulting container image is pushed.
layout: schema
name: BuildOutput
properties_list:
- description: Secret holding credentials for pushing to the output registry.
  name: pushSecret
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-output-schema.json
slug: openshift-rest-build-output
source_filename: openshift-rest-build-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildOutput\",\n  \"type\": \"object\",\n  \"description\": \"Specifies where the resulting container image is pushed.\",\n  \"properties\": {\n    \"pushSecret\": {\n      \"type\": \"object\",\n      \"description\": \"Secret holding credentials for pushing to the output registry.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-output-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildOutput
---
