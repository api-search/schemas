---
description: A document record in the Veeva Vault platform — a controlled document with lifecycle, version, and audit trail
layout: schema
name: Veeva Vault Document
properties_list:
- description: Unique Vault document ID
  name: id
  type: integer
- description: Document name (required)
  name: name__v
  type: string
- description: Document type API name (e.g., study_protocol__c)
  name: type__v
  type: string
- description: Document subtype API name
  name: subtype__v
  type: string
- description: Document classification API name
  name: classification__v
  type: string
- description: Document lifecycle API name (controls allowed states and actions)
  name: lifecycle__v
  type: string
- description: Current lifecycle state API name
  name: status__v
  type: string
- description: Auto-generated document number
  name: document_number__v
  type: string
- description: Major version number (increments on approval)
  name: major_version_number__v
  type: integer
- description: Minor version number (increments on draft revisions)
  name: minor_version_number__v
  type: integer
- description: User ID of document creator
  name: created_by__v
  type: integer
- description: User ID of last modifier
  name: last_modified_by__v
  type: integer
- description: Document creation timestamp
  name: created_date__v
  type: string
- description: Last modification timestamp
  name: last_modified_date__v
  type: string
- description: Document description
  name: description__v
  type: string
- description: Source file size in bytes
  name: size__v
  type: integer
- description: MIME type of source file (e.g., application/pdf)
  name: format__v
  type: string
- description: External system identifier for integration
  name: external_id__v
  type: string
- description: User ID of document owner
  name: owner__v
  type: integer
- description: User ID of document approver
  name: approver__v
  type: integer
- description: Date document becomes effective (approved state)
  name: effective_date__v
  type:
  - string
  - 'null'
- description: Document expiration date
  name: expiration_date__v
  type:
  - string
  - 'null'
provider_name: veeva
provider_slug: veeva
schema_file: json-schema/veeva-vault-document-schema.json
slug: veeva-vault-document
source_filename: veeva-vault-document-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.veevavault.com/schemas/document\",\n  \"title\": \"Veeva Vault Document\",\n  \"description\": \"A document record in the Veeva Vault platform — a controlled document with lifecycle, version, and audit trail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique Vault document ID\"\n    },\n    \"name__v\": {\n      \"type\": \"string\",\n      \"description\": \"Document name (required)\"\n    },\n    \"type__v\": {\n      \"type\": \"string\",\n      \"description\": \"Document type API name (e.g., study_protocol__c)\"\n    },\n    \"subtype__v\": {\n      \"type\": \"string\",\n      \"description\": \"Document subtype API name\"\n    },\n    \"classification__v\": {\n      \"type\": \"string\",\n      \"description\": \"Document classification API name\"\n    },\n    \"lifecycle__v\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Document lifecycle API name (controls allowed states and actions)\"\n    },\n    \"status__v\": {\n      \"type\": \"string\",\n      \"description\": \"Current lifecycle state API name\"\n    },\n    \"document_number__v\": {\n      \"type\": \"string\",\n      \"description\": \"Auto-generated document number\"\n    },\n    \"major_version_number__v\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Major version number (increments on approval)\"\n    },\n    \"minor_version_number__v\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Minor version number (increments on draft revisions)\"\n    },\n    \"created_by__v\": {\n      \"type\": \"integer\",\n      \"description\": \"User ID of document creator\"\n    },\n    \"last_modified_by__v\": {\n      \"type\": \"integer\",\n      \"description\": \"User ID of last modifier\"\n    },\n    \"created_date__v\": {\n      \"type\":\
  \ \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Document creation timestamp\"\n    },\n    \"last_modified_date__v\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Last modification timestamp\"\n    },\n    \"description__v\": {\n      \"type\": \"string\",\n      \"description\": \"Document description\"\n    },\n    \"size__v\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Source file size in bytes\"\n    },\n    \"format__v\": {\n      \"type\": \"string\",\n      \"description\": \"MIME type of source file (e.g., application/pdf)\"\n    },\n    \"external_id__v\": {\n      \"type\": \"string\",\n      \"description\": \"External system identifier for integration\"\n    },\n    \"owner__v\": {\n      \"type\": \"integer\",\n      \"description\": \"User ID of document owner\"\n    },\n    \"approver__v\": {\n      \"type\": \"integer\",\n      \"description\": \"User ID of document\
  \ approver\"\n    },\n    \"effective_date__v\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Date document becomes effective (approved state)\"\n    },\n    \"expiration_date__v\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Document expiration date\"\n    }\n  },\n  \"required\": [\"id\", \"name__v\", \"type__v\", \"lifecycle__v\", \"status__v\"],\n  \"additionalProperties\": {\n    \"description\": \"Custom field values (API names ending in __c)\"\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/veeva/refs/heads/main/json-schema/veeva-vault-document-schema.json
tags: []
title: Veeva Vault Document
---
