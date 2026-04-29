---
description: ''
layout: schema
name: Site
properties_list:
- description: The unique identifier for the site.
  name: id
  type: string
- description: The name of the site.
  name: name
  type: string
- description: The URL namespace for the site.
  name: contentUrl
  type: string
- description: The administrator mode for the site.
  name: adminMode
  type: string
- description: The current state of the site.
  name: state
  type: string
- description: The storage quota for the site in megabytes.
  name: storageQuota
  type: integer
- description: The maximum number of users for the site. A value of -1 indicates no limit.
  name: userQuota
  type: integer
- description: The number of Creator-licensed users on the site.
  name: numCreators
  type: integer
- description: The number of Explorer-licensed users on the site.
  name: numExplorers
  type: integer
- description: The number of Viewer-licensed users on the site.
  name: numViewers
  type: integer
- description: Whether subscriptions are disabled on the site.
  name: disableSubscriptions
  type: boolean
- description: The revision number of the site.
  name: revision
  type: string
- description: ''
  name: usage
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-site-schema.json
slug: tableau-rest-site
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Site\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the site.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the site.\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL namespace for the site.\"\n    },\n    \"adminMode\": {\n      \"type\": \"string\",\n      \"description\": \"The administrator mode for the site.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the site.\"\n    },\n    \"storageQuota\": {\n      \"type\": \"integer\",\n      \"description\": \"The storage quota for the site in megabytes.\"\n    },\n    \"userQuota\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of users for the site. A value of -1 indicates\
  \ no limit.\"\n    },\n    \"numCreators\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Creator-licensed users on the site.\"\n    },\n    \"numExplorers\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Explorer-licensed users on the site.\"\n    },\n    \"numViewers\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of Viewer-licensed users on the site.\"\n    },\n    \"disableSubscriptions\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether subscriptions are disabled on the site.\"\n    },\n    \"revision\": {\n      \"type\": \"string\",\n      \"description\": \"The revision number of the site.\"\n    },\n    \"usage\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-site-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Site
---
