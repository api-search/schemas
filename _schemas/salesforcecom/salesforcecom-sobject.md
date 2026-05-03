---
description: A Salesforce Standard or Custom Object record as returned by the Salesforce REST API
layout: schema
name: Salesforce sObject
properties_list:
- description: Unique 18-character Salesforce record ID
  name: Id
  type: string
- description: Name field of the record
  name: Name
  type: string
- description: Timestamp when the record was created
  name: CreatedDate
  type: string
- description: ID of the user who created the record
  name: CreatedById
  type: string
- description: Timestamp when the record was last modified
  name: LastModifiedDate
  type: string
- description: ID of the user who last modified the record
  name: LastModifiedById
  type: string
- description: ID of the user or queue who owns the record
  name: OwnerId
  type: string
- description: Whether the record has been soft-deleted (in recycle bin)
  name: IsDeleted
  type: boolean
- description: System timestamp of last modification including automated updates
  name: SystemModstamp
  type: string
- description: Salesforce metadata about the record including type and URL
  name: attributes
  type: object
provider_name: Salesforce
provider_slug: salesforcecom
schema_file: json-schema/salesforcecom-sobject-schema.json
slug: salesforcecom-sobject
source_filename: salesforcecom-sobject-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/salesforcecom/json-schema/salesforcecom-sobject-schema.json\",\n  \"title\": \"Salesforce sObject\",\n  \"description\": \"A Salesforce Standard or Custom Object record as returned by the Salesforce REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record ID\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name field of the record\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was created\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created the record\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the record was last modified\"\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified the record\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user or queue who owns the record\"\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record has been soft-deleted (in recycle bin)\"\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"System timestamp of last modification including automated updates\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Salesforce metadata about the record including type and URL\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"API name of the sObject type\
  \ (e.g. Account, Contact, Opportunity)\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"description\": \"REST API URL for this specific record\"\n        }\n      }\n    }\n  },\n  \"required\": [\"Id\", \"attributes\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforcecom/refs/heads/main/json-schema/salesforcecom-sobject-schema.json
tags:
- CRM
- Cloud
- Sales
- Marketing
- Automation
- AI
title: Salesforce sObject
---
