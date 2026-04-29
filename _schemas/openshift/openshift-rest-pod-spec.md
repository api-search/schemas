---
description: Specification of the desired behavior of a pod.
layout: schema
name: PodSpec
properties_list:
- description: List of containers in the pod.
  name: containers
  type: array
- description: List of initialization containers.
  name: initContainers
  type: array
- description: ''
  name: restartPolicy
  type: string
- description: Name of the ServiceAccount to use for the pod.
  name: serviceAccountName
  type: string
- description: ''
  name: nodeSelector
  type: object
- description: ''
  name: volumes
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-pod-spec-schema.json
slug: openshift-rest-pod-spec
source_filename: openshift-rest-pod-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PodSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification of the desired behavior of a pod.\",\n  \"properties\": {\n    \"containers\": {\n      \"type\": \"array\",\n      \"description\": \"List of containers in the pod.\"\n    },\n    \"initContainers\": {\n      \"type\": \"array\",\n      \"description\": \"List of initialization containers.\"\n    },\n    \"restartPolicy\": {\n      \"type\": \"string\"\n    },\n    \"serviceAccountName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the ServiceAccount to use for the pod.\"\n    },\n    \"nodeSelector\": {\n      \"type\": \"object\"\n    },\n    \"volumes\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-pod-spec-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: PodSpec
---
