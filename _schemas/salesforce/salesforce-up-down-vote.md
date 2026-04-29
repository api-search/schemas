---
description: ''
layout: schema
name: UpDownVote
properties_list:
- description: ''
  name: downVoteCount
  type: integer
- description: ''
  name: myVote
  type: string
- description: ''
  name: upVoteCount
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-up-down-vote-schema.json
slug: salesforce-up-down-vote
source_filename: salesforce-up-down-vote-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"downVoteCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"myVote\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"upVoteCount\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    }\n  },\n  \"required\": [\n    \"downVoteCount\",\n    \"myVote\",\n    \"upVoteCount\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpDownVote\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-up-down-vote-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: UpDownVote
---
