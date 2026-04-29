---
description: ''
layout: schema
name: Workbook
properties_list:
- description: The unique identifier for the workbook.
  name: id
  type: string
- description: The name of the workbook.
  name: name
  type: string
- description: A description of the workbook.
  name: description
  type: string
- description: The URL name of the workbook, used in URLs to access the workbook.
  name: contentUrl
  type: string
- description: The full URL to the workbook on the server.
  name: webpageUrl
  type: string
- description: Whether the workbook shows views as tabs.
  name: showTabs
  type: boolean
- description: The size of the workbook in bytes.
  name: size
  type: integer
- description: The date and time the workbook was created.
  name: createdAt
  type: string
- description: The date and time the workbook was last updated.
  name: updatedAt
  type: string
- description: Whether extracts in the workbook are encrypted.
  name: encryptExtracts
  type: string
- description: The ID of the default view in the workbook.
  name: defaultViewId
  type: string
- description: ''
  name: project
  type: object
- description: ''
  name: owner
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: views
  type: object
- description: ''
  name: usage
  type: object
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-workbook-schema.json
slug: tableau-rest-workbook
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Workbook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the workbook.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workbook.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the workbook.\"\n    },\n    \"contentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL name of the workbook, used in URLs to access the workbook.\"\n    },\n    \"webpageUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The full URL to the workbook on the server.\"\n    },\n    \"showTabs\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the workbook shows views as tabs.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"The size\
  \ of the workbook in bytes.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the workbook was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the workbook was last updated.\"\n    },\n    \"encryptExtracts\": {\n      \"type\": \"string\",\n      \"description\": \"Whether extracts in the workbook are encrypted.\"\n    },\n    \"defaultViewId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the default view in the workbook.\"\n    },\n    \"project\": {\n      \"type\": \"object\"\n    },\n    \"owner\": {\n      \"type\": \"object\"\n    },\n    \"tags\": {\n      \"type\": \"object\"\n    },\n    \"views\": {\n      \"type\": \"object\"\n    },\n    \"usage\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-workbook-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Workbook
---
