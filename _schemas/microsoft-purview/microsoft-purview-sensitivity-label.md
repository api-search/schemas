---
description: Represents a sensitivity label in the Microsoft Purview Information Protection service. Sensitivity labels classify and protect organizational data.
layout: schema
name: Microsoft Purview Sensitivity Label
properties_list:
- description: The unique identifier of the sensitivity label
  name: id
  type: string
- description: The name of the sensitivity label
  name: name
  type: string
- description: The description of the sensitivity label
  name: description
  type: string
- description: The color associated with the label
  name: color
  type: string
- description: The sensitivity order value, higher means more sensitive
  name: sensitivity
  type: integer
- description: The tooltip text shown to users
  name: tooltip
  type: string
- description: Whether the label is currently active
  name: isActive
  type: boolean
- description: Whether the label can be applied by users
  name: isAppliable
  type: boolean
- description: The content formats the label applies to
  name: contentFormats
  type: array
- description: Whether the label applies protection (encryption, rights management)
  name: hasProtection
  type: boolean
- description: The parent label (for sub-labels)
  name: parent
  type: object
provider_name: Microsoft Purview
provider_slug: microsoft-purview
schema_file: json-schema/microsoft-purview-sensitivity-label-schema.json
slug: microsoft-purview-sensitivity-label
source_filename: microsoft-purview-sensitivity-label-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/microsoft-purview/json-schema/microsoft-purview-sensitivity-label-schema.json\",\n  \"title\": \"Microsoft Purview Sensitivity Label\",\n  \"description\": \"Represents a sensitivity label in the Microsoft Purview Information Protection service. Sensitivity labels classify and protect organizational data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the sensitivity label\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the sensitivity label\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the sensitivity label\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"The color associated with the label\"\n    },\n\
  \    \"sensitivity\": {\n      \"type\": \"integer\",\n      \"description\": \"The sensitivity order value, higher means more sensitive\"\n    },\n    \"tooltip\": {\n      \"type\": \"string\",\n      \"description\": \"The tooltip text shown to users\"\n    },\n    \"isActive\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the label is currently active\"\n    },\n    \"isAppliable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the label can be applied by users\"\n    },\n    \"contentFormats\": {\n      \"type\": \"array\",\n      \"description\": \"The content formats the label applies to\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"hasProtection\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the label applies protection (encryption, rights management)\"\n    },\n    \"parent\": {\n      \"type\": \"object\",\n      \"description\": \"The parent label (for sub-labels)\",\n      \"properties\"\
  : {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-purview/refs/heads/main/json-schema/microsoft-purview-sensitivity-label-schema.json
tags:
- Compliance
- Data Catalog
- Data Classification
- Data Governance
- Data Loss Prevention
- Information Protection
title: Microsoft Purview Sensitivity Label
---
