---
description: Atlassian Document Format (ADF) representation of rich text content. ADF is a JSON-based format used in Jira Cloud REST API v3 for description, comment, and other rich text fields.
layout: schema
name: AtlassianDocumentFormat
properties_list:
- description: The root node type. Always doc.
  name: type
  type: string
- description: The ADF version. Currently 1.
  name: version
  type: integer
- description: The content nodes of the document.
  name: content
  type: array
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-atlassian-document-format-schema.json
slug: jira-cloud-platform-rest-atlassian-document-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AtlassianDocumentFormat\",\n  \"type\": \"object\",\n  \"description\": \"Atlassian Document Format (ADF) representation of rich text content. ADF is a JSON-based format used in Jira Cloud REST API v3 for description, comment, and other rich text fields.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The root node type. Always doc.\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The ADF version. Currently 1.\"\n    },\n    \"content\": {\n      \"type\": \"array\",\n      \"description\": \"The content nodes of the document.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-atlassian-document-format-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: AtlassianDocumentFormat
---
