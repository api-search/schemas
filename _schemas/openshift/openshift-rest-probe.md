---
description: Describes a health check to be performed against a container.
layout: schema
name: Probe
properties_list:
- description: ''
  name: httpGet
  type: object
- description: ''
  name: tcpSocket
  type: object
- description: ''
  name: exec
  type: object
- description: ''
  name: initialDelaySeconds
  type: integer
- description: ''
  name: periodSeconds
  type: integer
- description: ''
  name: timeoutSeconds
  type: integer
- description: ''
  name: successThreshold
  type: integer
- description: ''
  name: failureThreshold
  type: integer
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-probe-schema.json
slug: openshift-rest-probe
source_filename: openshift-rest-probe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Probe\",\n  \"type\": \"object\",\n  \"description\": \"Describes a health check to be performed against a container.\",\n  \"properties\": {\n    \"httpGet\": {\n      \"type\": \"object\"\n    },\n    \"tcpSocket\": {\n      \"type\": \"object\"\n    },\n    \"exec\": {\n      \"type\": \"object\"\n    },\n    \"initialDelaySeconds\": {\n      \"type\": \"integer\"\n    },\n    \"periodSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"timeoutSeconds\": {\n      \"type\": \"integer\"\n    },\n    \"successThreshold\": {\n      \"type\": \"integer\"\n    },\n    \"failureThreshold\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-probe-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: Probe
---
