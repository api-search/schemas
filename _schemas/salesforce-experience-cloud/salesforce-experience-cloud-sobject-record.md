---
description: Represents a Salesforce sObject record with its attributes and field values. The specific fields available depend on the sObject type and field-level security.
layout: schema
name: sObject Record
properties_list:
- description: Record metadata including sObject type and API URL
  name: attributes
  type: object
- description: The 18-character case-safe record ID
  name: Id
  type: string
- description: Name field of the record (if the sObject has a Name field)
  name: Name
  type: string
- description: When the record was created
  name: CreatedDate
  type: string
- description: ID of the user who created the record
  name: CreatedById
  type: string
- description: When the record was last modified
  name: LastModifiedDate
  type: string
- description: ID of the user who last modified the record
  name: LastModifiedById
  type: string
- description: System-maintained modification timestamp
  name: SystemModstamp
  type: string
- description: Whether the record has been moved to the Recycle Bin
  name: IsDeleted
  type: boolean
- description: ID of the record owner (user or queue)
  name: OwnerId
  type: string
- description: ID of the record type assigned to this record
  name: RecordTypeId
  type: string
provider_name: Salesforce Experience Cloud
provider_slug: salesforce-experience-cloud
schema_file: json-schema/salesforce-experience-cloud-sobject-record-schema.json
slug: salesforce-experience-cloud-sobject-record
source_filename: salesforce-experience-cloud-sobject-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/experience-cloud/sobject-record.json\",\n  \"title\": \"sObject Record\",\n  \"description\": \"Represents a Salesforce sObject record with its attributes and field values. The specific fields available depend on the sObject type and field-level security.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Record metadata including sObject type and API URL\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"API name of the sObject type (e.g., Account, Contact, CustomObject__c)\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"REST API URL for this record\"\n        }\n      },\n      \"required\": [\"type\", \"url\"]\n    },\n    \"Id\": {\n \
  \     \"type\": \"string\",\n      \"description\": \"The 18-character case-safe record ID\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name field of the record (if the sObject has a Name field)\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the record was created\"\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created the record\"\n    },\n    \"LastModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the record was last modified\"\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified the record\"\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"System-maintained modification\
  \ timestamp\"\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the record has been moved to the Recycle Bin\",\n      \"default\": false\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the record owner (user or queue)\"\n    },\n    \"RecordTypeId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the record type assigned to this record\"\n    }\n  },\n  \"required\": [\"attributes\", \"Id\"],\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-experience-cloud/refs/heads/main/json-schema/salesforce-experience-cloud-sobject-record-schema.json
tags:
- CMS
- Communities
- CRM
- Customer Portal
- Digital Experience
- Experience Cloud
- Partner Portal
title: sObject Record
---
