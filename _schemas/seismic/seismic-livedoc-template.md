---
description: A LiveDoc template in the Seismic platform used for dynamic document generation by merging data into predefined layouts.
layout: schema
name: Seismic LiveDoc Template
properties_list:
- description: Unique identifier of the template.
  name: id
  type: string
- description: Name of the template.
  name: name
  type: string
- description: Description of the template.
  name: description
  type: string
- description: Supported output formats for this template.
  name: outputFormats
  type: array
- description: ID of the folder containing this template.
  name: folderId
  type: string
- description: Number of input fields defined in the template.
  name: inputCount
  type: integer
- description: ID of the default data source for this template.
  name: dataSourceId
  type:
  - string
  - 'null'
- description: Status of the template.
  name: status
  type: string
- description: Input field definitions for the template.
  name: inputs
  type: array
- description: ID of the user who created the template.
  name: createdBy
  type: string
- description: Timestamp when the template was created.
  name: createdAt
  type: string
- description: ID of the user who last modified the template.
  name: modifiedBy
  type: string
- description: Timestamp when the template was last modified.
  name: modifiedAt
  type: string
- description: URL for the template thumbnail image.
  name: thumbnailUrl
  type: string
provider_name: Seismic
provider_slug: seismic
schema_file: json-schema/seismic-livedoc-template-schema.json
slug: seismic-livedoc-template
source_filename: seismic-livedoc-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.seismic.com/schemas/livedoc-template\",\n  \"title\": \"Seismic LiveDoc Template\",\n  \"description\": \"A LiveDoc template in the Seismic platform used for dynamic document generation by merging data into predefined layouts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the template.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the template.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the template.\"\n    },\n    \"outputFormats\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"pptx\", \"pdf\", \"docx\", \"xlsx\"]\n      },\n      \"description\": \"Supported output formats for this template.\"\n    },\n    \"folderId\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"ID of the folder containing this template.\"\n    },\n    \"inputCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of input fields defined in the template.\",\n      \"minimum\": 0\n    },\n    \"dataSourceId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"ID of the default data source for this template.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the template.\",\n      \"enum\": [\"active\", \"inactive\", \"draft\"]\n    },\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/TemplateInput\"\n      },\n      \"description\": \"Input field definitions for the template.\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created the template.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n  \
  \    \"description\": \"Timestamp when the template was created.\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified the template.\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the template was last modified.\"\n    },\n    \"thumbnailUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for the template thumbnail image.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"$defs\": {\n    \"TemplateInput\": {\n      \"type\": \"object\",\n      \"description\": \"An input field definition for a LiveDoc template.\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier of the input field.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the input field used as\
  \ key in generation requests.\"\n        },\n        \"displayName\": {\n          \"type\": \"string\",\n          \"description\": \"Display label for the input field.\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Data type of the input field.\",\n          \"enum\": [\"text\", \"number\", \"date\", \"boolean\", \"image\", \"table\", \"dropdown\"]\n        },\n        \"required\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the input field is required for generation.\"\n        },\n        \"defaultValue\": {\n          \"description\": \"Default value for the input field.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description or help text for the input field.\"\n        },\n        \"options\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"Available options\
  \ for dropdown-type inputs.\"\n        },\n        \"dataSourceField\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the data source field this input maps to for automatic population.\"\n        }\n      },\n      \"required\": [\"id\", \"name\", \"type\"]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/seismic/refs/heads/main/json-schema/seismic-livedoc-template-schema.json
tags: []
title: Seismic LiveDoc Template
---
