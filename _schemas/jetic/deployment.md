---
description: A Deployment represents a running instance of an integration on a connected Kubernetes cluster, managed through the Camel Bridge operator.
layout: schema
name: Jetic Deployment
properties_list:
- description: Unique deployment identifier.
  name: id
  type: string
- description: Associated integration identifier.
  name: integrationId
  type: string
- description: Name of the deployed integration.
  name: integrationName
  type: string
- description: Target cluster identifier.
  name: clusterId
  type: string
- description: Name of the target cluster.
  name: clusterName
  type: string
- description: Current deployment status.
  name: status
  type: string
- description: Target deployment environment.
  name: environment
  type: string
- description: Deployed version.
  name: version
  type: string
- description: Timestamp when the deployment was initiated.
  name: deployedAt
  type: string
- description: Timestamp when the deployment was last updated.
  name: updatedAt
  type: string
provider_name: Jetic
provider_slug: jetic
schema_file: json-schema/deployment.json
slug: deployment
source_filename: deployment.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/jetic/blob/main/json-schema/deployment.json\",\n  \"title\": \"Jetic Deployment\",\n  \"description\": \"A Deployment represents a running instance of an integration on a connected Kubernetes cluster, managed through the Camel Bridge operator.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique deployment identifier.\"\n    },\n    \"integrationId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated integration identifier.\"\n    },\n    \"integrationName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the deployed integration.\"\n    },\n    \"clusterId\": {\n      \"type\": \"string\",\n      \"description\": \"Target cluster identifier.\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target cluster.\"\
  \n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"running\",\n        \"building\",\n        \"stopped\",\n        \"error\"\n      ],\n      \"description\": \"Current deployment status.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"development\",\n        \"staging\",\n        \"production\"\n      ],\n      \"description\": \"Target deployment environment.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Deployed version.\"\n    },\n    \"deployedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was initiated.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was last updated.\"\n    }\n  },\n  \"required\": [\n    \"integrationId\",\n    \"clusterId\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetic/refs/heads/main/json-schema/deployment.json
tags:
- Apache Camel
- Integrations
- iPaaS
- Pro-Code API Composition
title: Jetic Deployment
---
