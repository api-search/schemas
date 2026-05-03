---
description: Represents a Prism Analytics dataset in Workday, used for loading external data into Workday for advanced reporting and analytics. Datasets have defined schemas and go through draft, upload, and publish lifecycle stages.
layout: schema
name: Workday Prism Analytics Dataset
properties_list:
- description: Workday ID of the dataset
  name: id
  type: string
- description: Name of the dataset
  name: name
  type: string
- description: Description of the dataset
  name: description
  type: string
- description: Current lifecycle status of the dataset
  name: status
  type: string
- description: Number of rows in the published dataset
  name: rowCount
  type: integer
- description: When the dataset was created
  name: createdDate
  type: string
- description: When the dataset was last modified
  name: modifiedDate
  type: string
- description: When the dataset was last published
  name: publishedDate
  type:
  - string
  - 'null'
- description: Field definitions for the dataset
  name: schema
  type: array
provider_name: Workday Integrations
provider_slug: workday-integrations
schema_file: json-schema/workday-integrations-dataset-schema.json
slug: workday-integrations-dataset
source_filename: workday-integrations-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://community.workday.com/schemas/workday-integrations/dataset.json\",\n  \"title\": \"Workday Prism Analytics Dataset\",\n  \"description\": \"Represents a Prism Analytics dataset in Workday, used for loading external data into Workday for advanced reporting and analytics. Datasets have defined schemas and go through draft, upload, and publish lifecycle stages.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Workday ID of the dataset\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the dataset\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the dataset\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Draft\"\
  , \"Published\", \"Publishing\", \"Failed\"],\n      \"description\": \"Current lifecycle status of the dataset\"\n    },\n    \"rowCount\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Number of rows in the published dataset\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the dataset was created\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the dataset was last modified\"\n    },\n    \"publishedDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"When the dataset was last published\"\n    },\n    \"schema\": {\n      \"type\": \"array\",\n      \"description\": \"Field definitions for the dataset\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/$defs/FieldDefinition\"\n      }\n    }\n  },\n  \"$defs\": {\n   \
  \ \"FieldDefinition\": {\n      \"type\": \"object\",\n      \"description\": \"Defines a field/column in a Prism Analytics dataset\",\n      \"required\": [\"name\", \"type\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Field name\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Field description\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\"Text\", \"Numeric\", \"Date\", \"Boolean\", \"Currency\"],\n          \"description\": \"Data type of the field\"\n        },\n        \"precision\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Decimal precision for numeric fields\"\n        },\n        \"isRequired\": {\n          \"type\": \"boolean\",\n          \"default\": false,\n          \"description\": \"Whether the field is required\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday-integrations/refs/heads/main/json-schema/workday-integrations-dataset-schema.json
tags:
- Cloud
- Enterprise Software
- ERP
- Finance
- HCM
- HR
- Integration
title: Workday Prism Analytics Dataset
---
