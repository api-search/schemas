---
description: An audit activity record from the Office 365 Management Activity API representing a user, admin, system, or policy action or event.
layout: schema
name: ActivityRecord
properties_list:
- description: The date and time in UTC when the user performed the activity.
  name: CreationTime
  type: string
- description: Unique identifier of an audit record.
  name: Id
  type: string
- description: The name of the user or admin activity.
  name: Operation
  type: string
- description: The GUID for the organization's tenant.
  name: OrganizationId
  type: string
- description: The type of operation indicated by the record.
  name: RecordType
  type: integer
- description: Indicates whether the action was successful or not.
  name: ResultStatus
  type: string
- description: A unique ID for the user identified in the UserId property.
  name: UserKey
  type: string
- description: The type of user that performed the operation.
  name: UserType
  type: integer
- description: The Office 365 service where the activity occurred.
  name: Workload
  type: string
- description: The IP address of the device used when the activity was logged.
  name: ClientIP
  type: string
- description: The object that was accessed or modified by the activity.
  name: ObjectId
  type: string
- description: The user who performed the action that resulted in the record being logged.
  name: UserId
  type: string
provider_name: Microsoft Office Integration
provider_slug: microsoft-office-integration
schema_file: json-schema/activity-record.json
slug: activity-record
source_filename: activity-record.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"activity-record.json\",\n  \"title\": \"ActivityRecord\",\n  \"description\": \"An audit activity record from the Office 365 Management Activity API representing a user, admin, system, or policy action or event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CreationTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time in UTC when the user performed the activity.\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier of an audit record.\"\n    },\n    \"Operation\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the user or admin activity.\"\n    },\n    \"OrganizationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The GUID for the organization's tenant.\"\n    },\n    \"RecordType\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"The type of operation indicated by the record.\"\n    },\n    \"ResultStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates whether the action was successful or not.\",\n      \"enum\": [\"success\", \"failed\", \"partiallySucceeded\"]\n    },\n    \"UserKey\": {\n      \"type\": \"string\",\n      \"description\": \"A unique ID for the user identified in the UserId property.\"\n    },\n    \"UserType\": {\n      \"type\": \"integer\",\n      \"description\": \"The type of user that performed the operation.\"\n    },\n    \"Workload\": {\n      \"type\": \"string\",\n      \"description\": \"The Office 365 service where the activity occurred.\"\n    },\n    \"ClientIP\": {\n      \"type\": \"string\",\n      \"description\": \"The IP address of the device used when the activity was logged.\"\n    },\n    \"ObjectId\": {\n      \"type\": \"string\",\n      \"description\": \"The object that was accessed or modified\
  \ by the activity.\"\n    },\n    \"UserId\": {\n      \"type\": \"string\",\n      \"description\": \"The user who performed the action that resulted in the record being logged.\"\n    }\n  },\n  \"required\": [\"CreationTime\", \"Id\", \"Operation\", \"OrganizationId\", \"RecordType\", \"UserId\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-office-integration/refs/heads/main/json-schema/activity-record.json
tags:
- Microsoft 365
- Microsoft Office Integration
- Office 365
title: ActivityRecord
---
