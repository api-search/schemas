---
description: Specification of the desired BuildConfig behavior.
layout: schema
name: BuildConfigSpec
properties_list:
- description: Triggers that cause new builds to be created.
  name: triggers
  type: array
- description: Controls how builds from this config run concurrently.
  name: runPolicy
  type: string
- description: The ServiceAccount to run the build pod as.
  name: serviceAccount
  type: string
- description: Optional duration in seconds builds may be active before being terminated.
  name: completionDeadlineSeconds
  type: integer
- description: Number of successful builds to retain.
  name: successfulBuildsHistoryLimit
  type: integer
- description: Number of failed builds to retain.
  name: failedBuildsHistoryLimit
  type: integer
- description: ''
  name: nodeSelector
  type: object
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-build-config-spec-schema.json
slug: openshift-rest-build-config-spec
source_filename: openshift-rest-build-config-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BuildConfigSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification of the desired BuildConfig behavior.\",\n  \"properties\": {\n    \"triggers\": {\n      \"type\": \"array\",\n      \"description\": \"Triggers that cause new builds to be created.\"\n    },\n    \"runPolicy\": {\n      \"type\": \"string\",\n      \"description\": \"Controls how builds from this config run concurrently.\"\n    },\n    \"serviceAccount\": {\n      \"type\": \"string\",\n      \"description\": \"The ServiceAccount to run the build pod as.\"\n    },\n    \"completionDeadlineSeconds\": {\n      \"type\": \"integer\",\n      \"description\": \"Optional duration in seconds builds may be active before being terminated.\"\n    },\n    \"successfulBuildsHistoryLimit\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of successful builds to retain.\"\n    },\n    \"failedBuildsHistoryLimit\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Number of failed builds to retain.\"\n    },\n    \"nodeSelector\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-build-config-spec-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: BuildConfigSpec
---
