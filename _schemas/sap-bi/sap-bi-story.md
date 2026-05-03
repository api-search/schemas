---
description: An analytics story in SAP Analytics Cloud that combines data visualizations, charts, tables, and other widgets into interactive dashboards and reports for data-driven decision making.
layout: schema
name: SAP Analytics Cloud Story
properties_list:
- description: Unique identifier for the story
  name: id
  type: string
- description: Name of the story
  name: name
  type: string
- description: Description of the story
  name: description
  type: string
- description: User who created the story
  name: createdBy
  type: string
- description: When the story was created
  name: createdTime
  type: string
- description: User who last modified the story
  name: modifiedBy
  type: string
- description: When the story was last modified
  name: modifiedTime
  type: string
- description: Current publication status of the story
  name: status
  type: string
- description: ID of the folder containing the story
  name: folderId
  type: string
- description: Pages within the story
  name: pages
  type: array
provider_name: SAP Business Intelligence
provider_slug: sap-bi
schema_file: json-schema/sap-bi-story-schema.json
slug: sap-bi-story
source_filename: sap-bi-story-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-bi/story.json\",\n  \"title\": \"SAP Analytics Cloud Story\",\n  \"description\": \"An analytics story in SAP Analytics Cloud that combines data visualizations, charts, tables, and other widgets into interactive dashboards and reports for data-driven decision making.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the story\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the story\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the story\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who created the story\"\n    },\n    \"createdTime\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the story was created\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"User who last modified the story\"\n    },\n    \"modifiedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the story was last modified\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Draft\", \"Published\"],\n      \"description\": \"Current publication status of the story\"\n    },\n    \"folderId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the folder containing the story\"\n    },\n    \"pages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Page\"\n      },\n      \"description\": \"Pages within the story\"\n    }\n  },\n  \"$defs\": {\n    \"Page\": {\n      \"type\": \"object\",\n      \"description\": \"A page within an analytics story containing one or more\
  \ widgets\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Page unique identifier\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Page name\"\n        },\n        \"widgets\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Widget\"\n          },\n          \"description\": \"Widgets on the page\"\n        }\n      }\n    },\n    \"Widget\": {\n      \"type\": \"object\",\n      \"description\": \"A visualization or interactive component on a story page\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Widget unique identifier\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"Chart\", \"Table\", \"Filter\", \"Text\", \"Image\", \"Shape\"],\n          \"description\": \"Type of widget\"\n        },\n        \"name\": {\n          \"type\"\
  : \"string\",\n          \"description\": \"Widget display name\"\n        },\n        \"modelId\": {\n          \"type\": \"string\",\n          \"description\": \"Associated data model ID\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/json-schema/sap-bi-story-schema.json
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
title: SAP Analytics Cloud Story
---
