---
description: A single application container running within a pod.
layout: schema
name: Container
properties_list:
- description: Name of the container.
  name: name
  type: string
- description: Container image name.
  name: image
  type: string
- description: Entrypoint array.
  name: command
  type: array
- description: Arguments to the entrypoint.
  name: args
  type: array
- description: ''
  name: env
  type: array
- description: ''
  name: ports
  type: array
- description: ''
  name: volumeMounts
  type: array
- description: ''
  name: imagePullPolicy
  type: string
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-container-schema.json
slug: openshift-rest-container
source_filename: openshift-rest-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Container\",\n  \"type\": \"object\",\n  \"description\": \"A single application container running within a pod.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the container.\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"description\": \"Container image name.\"\n    },\n    \"command\": {\n      \"type\": \"array\",\n      \"description\": \"Entrypoint array.\"\n    },\n    \"args\": {\n      \"type\": \"array\",\n      \"description\": \"Arguments to the entrypoint.\"\n    },\n    \"env\": {\n      \"type\": \"array\"\n    },\n    \"ports\": {\n      \"type\": \"array\"\n    },\n    \"volumeMounts\": {\n      \"type\": \"array\"\n    },\n    \"imagePullPolicy\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-container-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: Container
---
