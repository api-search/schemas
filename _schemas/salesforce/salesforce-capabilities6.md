---
description: ''
layout: schema
name: Capabilities6
properties_list:
- description: ''
  name: edit
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: upDownVote
  type: object
- description: ''
  name: verified
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-capabilities6-schema.json
slug: salesforce-capabilities6
source_filename: salesforce-capabilities6-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"edit\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isEditRestricted\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isEditableByMeUrl\": {\n          \"type\": \"string\",\n          \"example\": \"https://www.example.com\"\n        },\n        \"lastEditedBy\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"lastEditedDate\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"latestRevision\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"relativeLastEditedDate\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"isEditRestricted\",\n        \"isEditableByMeUrl\",\n        \"lastEditedBy\",\n      \
  \  \"lastEditedDate\",\n        \"latestRevision\",\n        \"relativeLastEditedDate\"\n      ]\n    },\n    \"status\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"feedEntityStatus\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"isApprovableByMe\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"feedEntityStatus\",\n        \"isApprovableByMe\"\n      ]\n    },\n    \"upDownVote\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"downVoteCount\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        },\n        \"myVote\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"upVoteCount\": {\n          \"type\": \"integer\",\n          \"example\": 42\n        }\n      },\n      \"required\": [\n        \"downVoteCount\",\n        \"myVote\",\n        \"\
  upVoteCount\"\n      ]\n    },\n    \"verified\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"isVerifiableByMe\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isVerified\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"isVerifiedByAnonymized\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"lastVerifiedByUser\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        },\n        \"lastVerifiedDate\": {\n          \"type\": \"['string', 'null']\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"isVerifiableByMe\",\n        \"isVerified\",\n        \"isVerifiedByAnonymized\",\n        \"lastVerifiedByUser\",\n        \"lastVerifiedDate\"\n      ]\n    }\n  },\n  \"required\": [\n    \"edit\",\n    \"status\",\n    \"upDownVote\"\
  ,\n    \"verified\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Capabilities6\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-capabilities6-schema.json
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
title: Capabilities6
---
