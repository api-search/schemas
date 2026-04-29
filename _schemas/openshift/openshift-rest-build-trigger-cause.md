---
description: Records which event triggered the build.
layout: schema
name: BuildTriggerCause
properties_list:
- description: Short human-readable description of the trigger.
  name: message
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-trigger-cause-schema.json
slug: openshift-rest-build-trigger-cause
source_filename: openshift-rest-build-trigger-cause-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildTriggerCause\",\n  \"type\": \"object\",\n  \"description\": \"Records which event triggered the build.\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Short human-readable description of the trigger.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-trigger-cause-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildTriggerCause
---
