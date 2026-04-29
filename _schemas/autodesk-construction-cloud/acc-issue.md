---
description: JSON Schema for an ACC construction issue, observation, or punch list item.
layout: schema
name: Autodesk Construction Cloud Issue
properties_list:
- description: Unique issue identifier (UUID)
  name: id
  type: string
- description: ACC project container identifier
  name: containerId
  type: string
- description: Human-readable sequential issue number
  name: displayId
  type: integer
- description: Issue title/summary
  name: title
  type: string
- description: Detailed issue description
  name: description
  type: string
- description: Current issue status
  name: status
  type: string
- description: Issue type identifier
  name: issueTypeId
  type: string
- description: Issue subtype identifier
  name: issueSubtypeId
  type: string
- description: ''
  name: dueDate
  type: string
- description: ''
  name: startDate
  type: string
- description: Location identifier within the project
  name: locationId
  type: string
- description: Free-text location description
  name: locationDescription
  type: string
- description: User or company assigned to resolve the issue
  name: assignedToId
  type: string
- description: ''
  name: assignedToType
  type: string
- description: User ID who created the issue
  name: createdBy
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
- description: ''
  name: closedBy
  type: string
- description: ''
  name: closedAt
  type: string
- description: ''
  name: rootCauseId
  type: string
- description: ''
  name: commentCount
  type: integer
- description: ''
  name: attachmentCount
  type: integer
- description: ''
  name: linkedDocuments
  type: array
provider_name: Autodesk Construction Cloud
provider_slug: autodesk-construction-cloud
schema_file: json-schema/acc-issue-schema.json
slug: acc-issue
source_filename: acc-issue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/json-schema/acc-issue-schema.json\",\n  \"title\": \"Autodesk Construction Cloud Issue\",\n  \"description\": \"JSON Schema for an ACC construction issue, observation, or punch list item.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"title\", \"status\", \"issueTypeId\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique issue identifier (UUID)\"\n    },\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"ACC project container identifier\"\n    },\n    \"displayId\": {\n      \"type\": \"integer\",\n      \"description\": \"Human-readable sequential issue number\",\n      \"minimum\": 1\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Issue title/summary\"\n    },\n    \"description\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Detailed issue description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"draft\", \"open\", \"pending\", \"in_review\", \"closed\"],\n      \"description\": \"Current issue status\"\n    },\n    \"issueTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"Issue type identifier\"\n    },\n    \"issueSubtypeId\": {\n      \"type\": \"string\",\n      \"description\": \"Issue subtype identifier\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"locationId\": {\n      \"type\": \"string\",\n      \"description\": \"Location identifier within the project\"\n    },\n    \"locationDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Free-text location description\"\n    },\n    \"assignedToId\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"User or company assigned to resolve the issue\"\n    },\n    \"assignedToType\": {\n      \"type\": \"string\",\n      \"enum\": [\"user\", \"company\"]\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User ID who created the issue\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"closedBy\": {\n      \"type\": \"string\"\n    },\n    \"closedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"rootCauseId\": {\n      \"type\": \"string\"\n    },\n    \"commentCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"attachmentCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0\n    },\n    \"linkedDocuments\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"urn\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"APS document URN\"\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/autodesk-construction-cloud/refs/heads/main/json-schema/acc-issue-schema.json
tags:
- Construction
- BIM
- Project Management
- AEC
- CAD
- Architecture
- Engineering
- Field Management
title: Autodesk Construction Cloud Issue
---
