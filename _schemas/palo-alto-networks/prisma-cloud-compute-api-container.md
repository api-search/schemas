---
description: Container schema from Palo Alto Networks Prisma Cloud Compute API
layout: schema
name: Container
properties_list:
- description: Unique container identifier.
  name: _id
  type: string
- description: Container name.
  name: name
  type: string
- description: Host where the container is running.
  name: hostname
  type: string
- description: ID of the container image.
  name: imageId
  type: string
- description: Full image name including registry, repository, and tag.
  name: imageName
  type: string
- description: Current container state.
  name: state
  type: string
- description: Container creation timestamp.
  name: created
  type: string
- description: Kubernetes cluster name.
  name: cluster
  type: string
- description: Kubernetes namespace.
  name: namespace
  type: string
- description: Number of vulnerabilities in the container image.
  name: vulnerabilitiesCount
  type: integer
- description: Number of compliance issues for this container.
  name: complianceIssuesCount
  type: integer
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-compute-api-container-schema.json
slug: prisma-cloud-compute-api-container
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Container\",\n  \"description\": \"Container schema from Palo Alto Networks Prisma Cloud Compute API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-container-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique container identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Container name.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Host where the container is running.\"\n    },\n    \"imageId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the container image.\"\n    },\n    \"imageName\": {\n      \"type\": \"string\",\n      \"description\": \"Full image name including registry, repository, and tag.\"\n    },\n    \"\
  state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"running\",\n        \"created\",\n        \"exited\",\n        \"paused\"\n      ],\n      \"description\": \"Current container state.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Container creation timestamp.\"\n    },\n    \"cluster\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes cluster name.\"\n    },\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"Kubernetes namespace.\"\n    },\n    \"vulnerabilitiesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of vulnerabilities in the container image.\"\n    },\n    \"complianceIssuesCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of compliance issues for this container.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-compute-api-container-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Container
---
