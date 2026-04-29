---
description: Standard Kubernetes object metadata. Every resource includes metadata such as name, namespace, labels, and annotations.
layout: schema
name: ObjectMeta
properties_list:
- description: The name of the resource, unique within a namespace.
  name: name
  type: string
- description: The namespace in which the resource resides.
  name: namespace
  type: string
- description: A unique identifier for the resource set by the server.
  name: uid
  type: string
- description: An opaque value representing the internal version of the object.
  name: resourceVersion
  type: string
- description: A sequence number representing a specific generation of the desired state.
  name: generation
  type: integer
- description: Timestamp representing when the object was created.
  name: creationTimestamp
  type: string
- description: Timestamp at which the object will be deleted.
  name: deletionTimestamp
  type: string
- description: Map of string keys and values that can be used to organize and categorize objects.
  name: labels
  type: object
- description: Unstructured key-value map stored with a resource for arbitrary metadata.
  name: annotations
  type: object
- description: List of objects depended by this object.
  name: ownerReferences
  type: array
- description: Must be empty before the object is deleted from the registry.
  name: finalizers
  type: array
provider_name: OpenShift
provider_slug: openshift
schema_file: json-schema/openshift-rest-object-meta-schema.json
slug: openshift-rest-object-meta
source_filename: openshift-rest-object-meta-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ObjectMeta\",\n  \"type\": \"object\",\n  \"description\": \"Standard Kubernetes object metadata. Every resource includes metadata such as name, namespace, labels, and annotations.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the resource, unique within a namespace.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace in which the resource resides.\"\n    },\n    \"uid\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the resource set by the server.\"\n    },\n    \"resourceVersion\": {\n      \"type\": \"string\",\n      \"description\": \"An opaque value representing the internal version of the object.\"\n    },\n    \"generation\": {\n      \"type\": \"integer\",\n      \"description\": \"A sequence number representing a specific generation of the\
  \ desired state.\"\n    },\n    \"creationTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp representing when the object was created.\"\n    },\n    \"deletionTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp at which the object will be deleted.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Map of string keys and values that can be used to organize and categorize objects.\"\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"description\": \"Unstructured key-value map stored with a resource for arbitrary metadata.\"\n    },\n    \"ownerReferences\": {\n      \"type\": \"array\",\n      \"description\": \"List of objects depended by this object.\"\n    },\n    \"finalizers\": {\n      \"type\": \"array\",\n      \"description\": \"Must be empty before the object is deleted from the registry.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/json-schema/openshift-rest-object-meta-schema.json
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
title: ObjectMeta
---
