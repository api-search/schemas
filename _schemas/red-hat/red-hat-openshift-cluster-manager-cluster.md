---
description: Represents an OpenShift cluster managed through the Cluster Manager.
layout: schema
name: Cluster
properties_list:
- description: The unique identifier of the cluster.
  name: id
  type: string
- description: The name of the cluster.
  name: name
  type: string
- description: The display name of the cluster.
  name: display_name
  type: string
- description: The current state of the cluster.
  name: state
  type: string
- description: The cloud provider where the cluster is deployed.
  name: cloud_provider
  type: object
- description: The cloud region where the cluster is deployed.
  name: region
  type: object
- description: Whether the cluster spans multiple availability zones for high availability.
  name: multi_az
  type: boolean
- description: Node configuration for the cluster.
  name: nodes
  type: object
- description: API server endpoint configuration.
  name: api
  type: object
- description: Web console configuration.
  name: console
  type: object
- description: The OpenShift version of the cluster.
  name: version
  type: object
- description: The date and time when the cluster was created.
  name: creation_timestamp
  type: string
- description: The date and time when the cluster is set to expire, if applicable.
  name: expiration_timestamp
  type: string
provider_name: Red Hat
provider_slug: red-hat
schema_file: json-schema/red-hat-openshift-cluster-manager-cluster-schema.json
slug: red-hat-openshift-cluster-manager-cluster
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Cluster\",\n  \"type\": \"object\",\n  \"description\": \"Represents an OpenShift cluster managed through the Cluster Manager.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cluster.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cluster.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the cluster.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the cluster.\"\n    },\n    \"cloud_provider\": {\n      \"type\": \"object\",\n      \"description\": \"The cloud provider where the cluster is deployed.\"\n    },\n    \"region\": {\n      \"type\": \"object\",\n      \"description\": \"The cloud region where the cluster is deployed.\"\n    },\n    \"multi_az\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the cluster spans multiple availability zones for high availability.\"\n    },\n    \"nodes\": {\n      \"type\": \"object\",\n      \"description\": \"Node configuration for the cluster.\"\n    },\n    \"api\": {\n      \"type\": \"object\",\n      \"description\": \"API server endpoint configuration.\"\n    },\n    \"console\": {\n      \"type\": \"object\",\n      \"description\": \"Web console configuration.\"\n    },\n    \"version\": {\n      \"type\": \"object\",\n      \"description\": \"The OpenShift version of the cluster.\"\n    },\n    \"creation_timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the cluster was created.\"\n    },\n    \"expiration_timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the cluster is set to expire, if applicable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/json-schema/red-hat-openshift-cluster-manager-cluster-schema.json
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
title: Cluster
---
