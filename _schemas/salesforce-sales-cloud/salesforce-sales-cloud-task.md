---
description: Represents a business activity such as making a phone call or other to-do items. Tasks can be associated with leads, accounts, contacts, opportunities, and other records. In the user interface, Task and Event records are collectively referred to as activities.
layout: schema
name: Salesforce Task
properties_list:
- description: Unique 18-character Salesforce record identifier
  name: Id
  type: string
- description: The ID of a related Contact or Lead
  name: WhoId
  type:
  - string
  - 'null'
- description: The ID of a related Account, Opportunity, Campaign, Case, or custom object
  name: WhatId
  type:
  - string
  - 'null'
- description: Subject line of the task
  name: Subject
  type:
  - string
  - 'null'
- description: Due date of the task
  name: ActivityDate
  type:
  - string
  - 'null'
- description: Status of the task
  name: Status
  type: string
- description: Priority of the task
  name: Priority
  type: string
- description: Indicates whether the task is high priority
  name: IsHighPriority
  type: boolean
- description: ID of the user or queue that owns the task
  name: OwnerId
  type: string
- description: Contains a text description of the task
  name: Description
  type:
  - string
  - 'null'
- description: Indicates whether the record has been moved to the Recycle Bin
  name: IsDeleted
  type: boolean
- description: Represents the ID of the related Account
  name: AccountId
  type:
  - string
  - 'null'
- description: Indicates whether the task has been completed
  name: IsClosed
  type: boolean
- description: Date and time when this record was created
  name: CreatedDate
  type: string
- description: ID of the user who created this record
  name: CreatedById
  type: string
- description: Date and time when this record was last modified
  name: LastModifiedDate
  type: string
- description: ID of the user who last modified this record
  name: LastModifiedById
  type: string
- description: ''
  name: SystemModstamp
  type: string
- description: Indicates whether the task has been archived
  name: IsArchived
  type: boolean
- description: Duration of the call in seconds, if this task is a call
  name: CallDurationInSeconds
  type:
  - integer
  - 'null'
- description: Type of call being tracked
  name: CallType
  type:
  - string
  - 'null'
- description: Result of a given call
  name: CallDisposition
  type:
  - string
  - 'null'
- description: Identifier for the call
  name: CallObject
  type:
  - string
  - 'null'
- description: Date and time to show a reminder
  name: ReminderDateTime
  type:
  - string
  - 'null'
- description: Indicates whether a reminder is set for this task
  name: IsReminderSet
  type: boolean
- description: The recurrence activity ID for the recurring series
  name: RecurrenceActivityId
  type:
  - string
  - 'null'
- description: Indicates whether the task is set to recur
  name: IsRecurrence
  type: boolean
- description: Provides classification for tasks
  name: TaskSubtype
  type:
  - string
  - 'null'
- description: Date and time the task was completed
  name: CompletedDateTime
  type:
  - string
  - 'null'
- description: ''
  name: attributes
  type: object
provider_name: Salesforce Sales Cloud
provider_slug: salesforce-sales-cloud
schema_file: json-schema/salesforce-sales-cloud-task-schema.json
slug: salesforce-sales-cloud-task
source_filename: salesforce-sales-cloud-task-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.salesforce.com/schemas/sales-cloud/task.json\",\n  \"title\": \"Salesforce Task\",\n  \"description\": \"Represents a business activity such as making a phone call or other to-do items. Tasks can be associated with leads, accounts, contacts, opportunities, and other records. In the user interface, Task and Event records are collectively referred to as activities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique 18-character Salesforce record identifier\",\n      \"pattern\": \"^[a-zA-Z0-9]{18}$\",\n      \"readOnly\": true\n    },\n    \"WhoId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of a related Contact or Lead\"\n    },\n    \"WhatId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The ID of a related Account, Opportunity, Campaign, Case,\
  \ or custom object\"\n    },\n    \"Subject\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Subject line of the task\",\n      \"maxLength\": 255\n    },\n    \"ActivityDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\",\n      \"description\": \"Due date of the task\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the task\",\n      \"enum\": [\"Not Started\", \"In Progress\", \"Completed\", \"Waiting on someone else\", \"Deferred\"]\n    },\n    \"Priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority of the task\",\n      \"enum\": [\"High\", \"Normal\", \"Low\"]\n    },\n    \"IsHighPriority\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the task is high priority\",\n      \"readOnly\": true\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user or queue that owns the task\"\n    },\n    \"\
  Description\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Contains a text description of the task\"\n    },\n    \"IsDeleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the record has been moved to the Recycle Bin\",\n      \"readOnly\": true\n    },\n    \"AccountId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Represents the ID of the related Account\",\n      \"readOnly\": true\n    },\n    \"IsClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the task has been completed\",\n      \"readOnly\": true\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was created\",\n      \"readOnly\": true\n    },\n    \"CreatedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who created this record\",\n      \"readOnly\": true\n    },\n    \"LastModifiedDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date and time when this record was last modified\",\n      \"readOnly\": true\n    },\n    \"LastModifiedById\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who last modified this record\",\n      \"readOnly\": true\n    },\n    \"SystemModstamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true\n    },\n    \"IsArchived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the task has been archived\",\n      \"readOnly\": true\n    },\n    \"CallDurationInSeconds\": {\n      \"type\": [\"integer\", \"null\"],\n      \"description\": \"Duration of the call in seconds, if this task is a call\"\n    },\n    \"CallType\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Type of call being tracked\",\n      \"enum\": [null, \"Internal\", \"Inbound\", \"Outbound\"]\n    },\n    \"CallDisposition\"\
  : {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Result of a given call\",\n      \"maxLength\": 255\n    },\n    \"CallObject\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Identifier for the call\",\n      \"maxLength\": 255\n    },\n    \"ReminderDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time to show a reminder\"\n    },\n    \"IsReminderSet\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether a reminder is set for this task\",\n      \"default\": false\n    },\n    \"RecurrenceActivityId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The recurrence activity ID for the recurring series\",\n      \"readOnly\": true\n    },\n    \"IsRecurrence\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the task is set to recur\",\n      \"readOnly\": true\n    },\n    \"TaskSubtype\": {\n\
  \      \"type\": [\"string\", \"null\"],\n      \"description\": \"Provides classification for tasks\",\n      \"enum\": [null, \"Task\", \"Email\", \"ListEmail\", \"Cadence\", \"Call\"]\n    },\n    \"CompletedDateTime\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Date and time the task was completed\",\n      \"readOnly\": true\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"Task\"\n        },\n        \"url\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\"Status\", \"Priority\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-sales-cloud/refs/heads/main/json-schema/salesforce-sales-cloud-task-schema.json
tags:
- Cloud
- CRM
- Customer Management
- Enterprise
- Sales
title: Salesforce Task
---
