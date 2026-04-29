---
description: The votes for an issue.
layout: schema
name: Votes
properties_list:
- description: ''
  name: self
  type: string
- description: ''
  name: votes
  type: integer
- description: ''
  name: hasVoted
  type: boolean
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-votes-schema.json
slug: jira-cloud-platform-rest-votes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Votes\",\n  \"type\": \"object\",\n  \"description\": \"The votes for an issue.\",\n  \"properties\": {\n    \"self\": {\n      \"type\": \"string\"\n    },\n    \"votes\": {\n      \"type\": \"integer\"\n    },\n    \"hasVoted\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-votes-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: Votes
---
