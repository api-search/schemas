---
description: Schema for an OpenShift Project resource. Projects are OpenShift's tenant wrapper around Kubernetes namespaces with additional RBAC and metadata.
layout: schema
name: Red Hat OpenShift Project
properties_list:
- description: OpenShift project API version
  name: apiVersion
  type: string
- description: Resource kind
  name: kind
  type: string
- description: ''
  name: metadata
  type: object
- description: ''
  name: spec
  type: object
- description: ''
  name: status
  type: object
provider_name: Red Hat OpenShift
provider_slug: red-hat-openshift
schema_file: json-schema/red-hat-openshift-project-schema.json
slug: red-hat-openshift-project
source_filename: red-hat-openshift-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/red-hat-openshift/json-schema/red-hat-openshift-project-schema.json\",\n  \"title\": \"Red Hat OpenShift Project\",\n  \"description\": \"Schema for an OpenShift Project resource. Projects are OpenShift's tenant wrapper around Kubernetes namespaces with additional RBAC and metadata.\",\n  \"type\": \"object\",\n  \"required\": [\"apiVersion\", \"kind\", \"metadata\"],\n  \"properties\": {\n    \"apiVersion\": {\n      \"type\": \"string\",\n      \"const\": \"project.openshift.io/v1\",\n      \"description\": \"OpenShift project API version\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"const\": \"Project\",\n      \"description\": \"Resource kind\"\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Project name (must be unique in the cluster)\",\n          \"pattern\": \"^[a-z0-9]([a-z0-9-]*[a-z0-9])?$\",\n          \"maxLength\": 63\n        },\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"System-generated unique identifier\"\n        },\n        \"resourceVersion\": {\n          \"type\": \"string\",\n          \"description\": \"Resource version for optimistic concurrency\"\n        },\n        \"creationTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Project creation timestamp\"\n        },\n        \"labels\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value labels for selection and filtering\",\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        },\n        \"annotations\": {\n          \"type\": \"object\",\n          \"description\": \"Non-identifying metadata annotations\",\n          \"properties\"\
  : {\n            \"openshift.io/description\": {\n              \"type\": \"string\",\n              \"description\": \"Human-readable project description\"\n            },\n            \"openshift.io/display-name\": {\n              \"type\": \"string\",\n              \"description\": \"Display name for the project in the console\"\n            },\n            \"openshift.io/requester\": {\n              \"type\": \"string\",\n              \"description\": \"Username of the project creator\"\n            }\n          },\n          \"additionalProperties\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"spec\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"finalizers\": {\n          \"type\": \"array\",\n          \"description\": \"Finalizers to run before project deletion\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"status\": {\n      \"type\": \"object\",\n   \
  \   \"properties\": {\n        \"phase\": {\n          \"type\": \"string\",\n          \"enum\": [\"Active\", \"Terminating\"],\n          \"description\": \"Project lifecycle phase\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/json-schema/red-hat-openshift-project-schema.json
tags:
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- PaaS
- Red Hat
title: Red Hat OpenShift Project
---
