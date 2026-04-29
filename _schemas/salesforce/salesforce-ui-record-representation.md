---
description: A Salesforce record with field values and UI metadata
layout: schema
name: RecordRepresentation
properties_list:
- description: The 18-character Salesforce record ID
  name: id
  type: string
- description: The API name of the object type
  name: apiName
  type: string
- description: Child relationship data indexed by relationship name
  name: childRelationships
  type: object
- description: ETag for optimistic concurrency control
  name: eTag
  type: string
- description: Field values indexed by field API name
  name: fields
  type: object
- description: The record type ID
  name: recordTypeId
  type: string
- description: Record type metadata
  name: recordTypeInfo
  type: object
- description: ''
  name: systemModstamp
  type: string
- description: ''
  name: lastModifiedById
  type: string
- description: ''
  name: lastModifiedDate
  type: string
- description: ''
  name: createdById
  type: string
- description: ''
  name: createdDate
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-record-representation-schema.json
slug: salesforce-ui-record-representation
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A Salesforce record with field values and UI metadata\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The 18-character Salesforce record ID\",\n      \"example\": \"abc123\"\n    },\n    \"apiName\": {\n      \"type\": \"string\",\n      \"description\": \"The API name of the object type\",\n      \"example\": \"example_value\"\n    },\n    \"childRelationships\": {\n      \"type\": \"object\",\n      \"description\": \"Child relationship data indexed by relationship name\",\n      \"example\": \"example_value\"\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"description\": \"ETag for optimistic concurrency control\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Field values indexed by field API name\",\n      \"example\": \"example_value\"\n    },\n    \"recordTypeId\": {\n      \"type\": \"\
  string\",\n      \"description\": \"The record type ID\",\n      \"example\": \"500123\"\n    },\n    \"recordTypeInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Record type metadata\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"available\": {\n          \"type\": \"boolean\"\n        },\n        \"defaultRecordTypeMapping\": {\n          \"type\": \"boolean\"\n        },\n        \"master\": {\n          \"type\": \"boolean\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"recordTypeId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"systemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    },\n    \"lastModifiedById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"lastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"\
  2026-01-15T10:30:00Z\"\n    },\n    \"createdById\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecordRepresentation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-record-representation-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: RecordRepresentation
---
