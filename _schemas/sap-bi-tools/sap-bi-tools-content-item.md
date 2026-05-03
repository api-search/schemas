---
description: Represents a content item in the SAP Analytics Cloud Content Network. Content items are shareable analytics artifacts such as stories, models, and packages.
layout: schema
name: SAP Analytics Cloud Content Item
properties_list:
- description: The unique identifier of the content item
  name: id
  type: string
- description: The display name of the content item
  name: name
  type: string
- description: A text description of the content item
  name: description
  type: string
- description: The type of content item
  name: type
  type: string
- description: The visibility scope
  name: visibility
  type: string
- description: The version of the content item
  name: version
  type: string
- description: The timestamp when the item was published
  name: createdTime
  type: string
- description: The timestamp when the item was last modified
  name: modifiedTime
  type: string
- description: The tenant that published the content item
  name: owner
  type: string
provider_name: SAP BI Tools
provider_slug: sap-bi-tools
schema_file: json-schema/sap-bi-tools-content-item-schema.json
slug: sap-bi-tools-content-item
source_filename: sap-bi-tools-content-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/sap-bi-tools/json-schema/sap-bi-tools-content-item-schema.json\",\n  \"title\": \"SAP Analytics Cloud Content Item\",\n  \"description\": \"Represents a content item in the SAP Analytics Cloud Content Network. Content items are shareable analytics artifacts such as stories, models, and packages.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the content item\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the content item\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A text description of the content item\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of content item\",\n      \"enum\": [\"STORY\", \"MODEL\", \"PACKAGE\"]\n   \
  \ },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"description\": \"The visibility scope\",\n      \"enum\": [\"PRIVATE\", \"PUBLIC\"]\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the content item\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the item was published\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the item was last modified\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The tenant that published the content item\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/json-schema/sap-bi-tools-content-item-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
title: SAP Analytics Cloud Content Item
---
