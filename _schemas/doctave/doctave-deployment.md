---
description: A deployment record for a Doctave documentation site, representing a build and publish operation triggered by a commit or manual action.
layout: schema
name: Doctave Deployment
properties_list:
- description: Unique identifier for the deployment.
  name: id
  type: string
- description: Identifier of the site this deployment belongs to.
  name: siteId
  type: string
- description: Current status of the deployment.
  name: status
  type: string
- description: Git commit SHA that triggered the deployment.
  name: commitSha
  type: string
- description: Git branch used for this deployment.
  name: branch
  type: string
- description: User or system that triggered the deployment.
  name: triggeredBy
  type: string
- description: Target environment for the deployment.
  name: environment
  type: string
- description: Duration of the build step in seconds.
  name: buildDuration
  type: integer
- description: Duration of the deploy step in seconds.
  name: deployDuration
  type: integer
- description: URL to the build log for this deployment.
  name: buildLog
  type: string
- description: URL where the deployed documentation is accessible.
  name: url
  type: string
- description: Timestamp when the deployment was created.
  name: createdAt
  type: string
- description: Timestamp when the deployment finished.
  name: finishedAt
  type: string
provider_name: Doctave
provider_slug: doctave
schema_file: json-schema/doctave-deployment-schema.json
slug: doctave-deployment
source_filename: doctave-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/json-schema/doctave-deployment-schema.json\",\n  \"title\": \"Doctave Deployment\",\n  \"description\": \"A deployment record for a Doctave documentation site, representing a build and publish operation triggered by a commit or manual action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the deployment.\"\n    },\n    \"siteId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the site this deployment belongs to.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"building\", \"deploying\", \"live\", \"failed\"],\n      \"description\": \"Current status of the deployment.\"\n    },\n    \"commitSha\": {\n      \"type\": \"string\",\n      \"description\": \"Git commit\
  \ SHA that triggered the deployment.\",\n      \"pattern\": \"^[0-9a-f]{40}$\"\n    },\n    \"branch\": {\n      \"type\": \"string\",\n      \"description\": \"Git branch used for this deployment.\"\n    },\n    \"triggeredBy\": {\n      \"type\": \"string\",\n      \"description\": \"User or system that triggered the deployment.\"\n    },\n    \"environment\": {\n      \"type\": \"string\",\n      \"enum\": [\"production\", \"staging\", \"preview\"],\n      \"description\": \"Target environment for the deployment.\"\n    },\n    \"buildDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of the build step in seconds.\"\n    },\n    \"deployDuration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of the deploy step in seconds.\"\n    },\n    \"buildLog\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the build log for this deployment.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n \
  \     \"format\": \"uri\",\n      \"description\": \"URL where the deployed documentation is accessible.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment was created.\"\n    },\n    \"finishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the deployment finished.\"\n    }\n  },\n  \"required\": [\"id\", \"siteId\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/doctave/refs/heads/main/json-schema/doctave-deployment-schema.json
tags:
- Documentation
- OpenAPI
- Platform
- Portals
title: Doctave Deployment
---
