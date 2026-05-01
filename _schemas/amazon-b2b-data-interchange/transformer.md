---
description: Represents a B2B Data Interchange transformer — defines how X12 EDI documents are converted to and from JSON or XML using mapping templates.
layout: schema
name: Transformer
properties_list:
- description: Unique identifier for the transformer
  name: transformerId
  type: string
- description: Amazon Resource Name (ARN) for the transformer
  name: transformerArn
  type: string
- description: Name of the transformer
  name: name
  type: string
- description: Current status of the transformer
  name: status
  type: string
- description: Output file format for the transformer
  name: fileFormat
  type: string
- description: JSONata or XSLT mapping template content
  name: mappingTemplate
  type: string
- description: EDI type configuration for the transformer
  name: ediType
  type: object
- description: Timestamp when the transformer was created
  name: createdAt
  type: string
- description: Timestamp when the transformer was last modified
  name: modifiedAt
  type: string
provider_name: Amazon B2B Data Interchange
provider_slug: amazon-b2b-data-interchange
schema_file: json-schema/transformer.json
slug: transformer
source_filename: transformer.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/main/json-schema/transformer.json\",\n  \"title\": \"Transformer\",\n  \"description\": \"Represents a B2B Data Interchange transformer — defines how X12 EDI documents are converted to and from JSON or XML using mapping templates.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transformerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the transformer\",\n      \"pattern\": \"^tr-[a-zA-Z0-9]+$\"\n    },\n    \"transformerArn\": {\n      \"type\": \"string\",\n      \"description\": \"Amazon Resource Name (ARN) for the transformer\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the transformer\",\n      \"minLength\": 1,\n      \"maxLength\": 254\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"\
  inactive\"],\n      \"description\": \"Current status of the transformer\"\n    },\n    \"fileFormat\": {\n      \"type\": \"string\",\n      \"enum\": [\"XML\", \"JSON\", \"NOT_USED\"],\n      \"description\": \"Output file format for the transformer\"\n    },\n    \"mappingTemplate\": {\n      \"type\": \"string\",\n      \"description\": \"JSONata or XSLT mapping template content\"\n    },\n    \"ediType\": {\n      \"type\": \"object\",\n      \"description\": \"EDI type configuration for the transformer\",\n      \"properties\": {\n        \"x12Details\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"transactionSet\": {\n              \"type\": \"string\",\n              \"description\": \"X12 transaction set (e.g. X12_850, X12_856, X12_810)\"\n            },\n            \"version\": {\n              \"type\": \"string\",\n              \"description\": \"X12 version (e.g. VERSION_4010, VERSION_5010)\"\n            }\n          }\n        }\n    \
  \  }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the transformer was created\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the transformer was last modified\"\n    }\n  },\n  \"required\": [\"transformerId\", \"transformerArn\", \"name\", \"status\", \"createdAt\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-b2b-data-interchange/refs/heads/main/json-schema/transformer.json
tags:
- EDI
- B2B
- Data Interchange
- Supply Chain
- Healthcare
- Financial Services
- Amazon Web Services
title: Transformer
---
