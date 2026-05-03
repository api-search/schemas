---
description: Schema for a public comment submitted to a regulatory docket via Regulations.gov.
layout: schema
name: Public Comment
properties_list:
- description: Unique identifier for the public comment.
  name: commentId
  type: string
- description: Regulatory docket this comment belongs to.
  name: docketId
  type: string
- description: Specific regulatory document being commented on.
  name: documentId
  type: string
- description: Date and time the comment was submitted.
  name: submittedDate
  type: string
- description: Date and time the comment was posted publicly.
  name: postedDate
  type: string
- description: Name of the person or organization submitting the comment.
  name: commenterName
  type: string
- description: Type of commenter.
  name: commenterType
  type: string
- description: Full text of the public comment.
  name: comment
  type: string
- description: Files attached to the comment.
  name: attachments
  type: array
- description: Agency that received the comment.
  name: agencyId
  type: string
provider_name: Regulation
provider_slug: regulation
schema_file: json-schema/regulation-comment-schema.json
slug: regulation-comment
source_filename: regulation-comment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/regulation/json-schema/regulation-comment-schema.json\",\n  \"title\": \"Public Comment\",\n  \"description\": \"Schema for a public comment submitted to a regulatory docket via Regulations.gov.\",\n  \"type\": \"object\",\n  \"required\": [\"commentId\", \"docketId\", \"submittedDate\"],\n  \"properties\": {\n    \"commentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the public comment.\"\n    },\n    \"docketId\": {\n      \"type\": \"string\",\n      \"description\": \"Regulatory docket this comment belongs to.\"\n    },\n    \"documentId\": {\n      \"type\": \"string\",\n      \"description\": \"Specific regulatory document being commented on.\"\n    },\n    \"submittedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the comment was submitted.\"\n    },\n\
  \    \"postedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the comment was posted publicly.\"\n    },\n    \"commenterName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the person or organization submitting the comment.\"\n    },\n    \"commenterType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of commenter.\",\n      \"enum\": [\"Individual\", \"Organization\", \"Anonymous\", \"Government\"]\n    },\n    \"comment\": {\n      \"type\": \"string\",\n      \"description\": \"Full text of the public comment.\"\n    },\n    \"attachments\": {\n      \"type\": \"array\",\n      \"description\": \"Files attached to the comment.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"fileUrl\": {\n            \"type\": \"string\",\n            \"format\": \"uri\"\n          },\n          \"fileFormat\": {\n            \"type\": \"string\"\n      \
  \    },\n          \"title\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"agencyId\": {\n      \"type\": \"string\",\n      \"description\": \"Agency that received the comment.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/regulation/refs/heads/main/json-schema/regulation-comment-schema.json
tags:
- Compliance
- Governance
- Government
- Legal
- Policy
- Regulation
- Regulatory Change
- Risk Management
title: Public Comment
---
