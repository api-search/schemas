---
description: Information protection sensitivity label applied to the document.
layout: schema
name: SensitivityLabel
properties_list:
- description: The unique identifier of the sensitivity label.
  name: sensitivityLabelId
  type: string
- description: The display name of the sensitivity label.
  name: displayName
  type: string
- description: Tooltip text describing the sensitivity label.
  name: toolTip
  type: string
- description: The priority of the sensitivity label.
  name: priority
  type: integer
- description: The color code associated with the sensitivity label.
  name: color
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-sensitivity-label-schema.json
slug: microsoft-copilot-sensitivity-label
source_filename: microsoft-copilot-sensitivity-label-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SensitivityLabel\",\n  \"type\": \"object\",\n  \"description\": \"Information protection sensitivity label applied to the document.\",\n  \"properties\": {\n    \"sensitivityLabelId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the sensitivity label.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the sensitivity label.\"\n    },\n    \"toolTip\": {\n      \"type\": \"string\",\n      \"description\": \"Tooltip text describing the sensitivity label.\"\n    },\n    \"priority\": {\n      \"type\": \"integer\",\n      \"description\": \"The priority of the sensitivity label.\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"The color code associated with the sensitivity label.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-sensitivity-label-schema.json
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
title: SensitivityLabel
---
