---
description: Schema for an Oracle Primavera P6 schedule activity, representing a work item within a project WBS.
layout: schema
name: Oracle Primavera P6 Activity
properties_list:
- description: System-generated unique identifier
  name: ObjectId
  type: integer
- description: User-defined activity ID
  name: Id
  type: string
- description: Activity name
  name: Name
  type: string
- description: Parent project ObjectId
  name: ProjectObjectId
  type: integer
- description: Parent WBS element ObjectId
  name: WBSObjectId
  type: integer
- description: Activity type
  name: Type
  type: string
- description: Current activity status
  name: Status
  type: string
- description: Activity percent complete
  name: PercentComplete
  type: number
- description: Method for calculating percent complete
  name: PercentCompleteType
  type: string
- description: ''
  name: PlannedStartDate
  type: string
- description: ''
  name: PlannedFinishDate
  type: string
- description: ''
  name: ActualStartDate
  type:
  - string
  - 'null'
- description: ''
  name: ActualFinishDate
  type:
  - string
  - 'null'
- description: ''
  name: RemainingStartDate
  type:
  - string
  - 'null'
- description: ''
  name: RemainingFinishDate
  type:
  - string
  - 'null'
- description: Planned duration in hours
  name: PlannedDuration
  type: number
- description: Actual duration accrued in hours
  name: ActualDuration
  type: number
- description: Remaining duration in hours
  name: RemainingDuration
  type: number
- description: Total float in hours; negative values indicate critical path
  name: TotalFloat
  type: number
- description: Free float in hours
  name: FreeFloat
  type: number
- description: True if activity is on the critical path
  name: CriticalFlag
  type: boolean
- description: Assigned work calendar ObjectId
  name: CalendarObjectId
  type: integer
- description: ''
  name: PrimaryConstraintType
  type: string
- description: ''
  name: PrimaryConstraintDate
  type:
  - string
  - 'null'
provider_name: Oracle Primavera
provider_slug: oracle-primavera
schema_file: json-schema/oracle-primavera-activity-schema.json
slug: oracle-primavera-activity
source_filename: oracle-primavera-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/oracle-primavera/json-schema/oracle-primavera-activity-schema.json\",\n  \"title\": \"Oracle Primavera P6 Activity\",\n  \"description\": \"Schema for an Oracle Primavera P6 schedule activity, representing a work item within a project WBS.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObjectId\": {\n      \"type\": \"integer\",\n      \"description\": \"System-generated unique identifier\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"User-defined activity ID\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"maxLength\": 120,\n      \"description\": \"Activity name\"\n    },\n    \"ProjectObjectId\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent project ObjectId\"\n    },\n    \"WBSObjectId\": {\n      \"type\": \"integer\",\n      \"description\": \"Parent WBS\
  \ element ObjectId\"\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Task Dependent\",\n        \"Resource Dependent\",\n        \"Level of Effort\",\n        \"Start Milestone\",\n        \"Finish Milestone\",\n        \"WBS Summary\"\n      ],\n      \"description\": \"Activity type\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Not Started\", \"In Progress\", \"Completed\"],\n      \"description\": \"Current activity status\"\n    },\n    \"PercentComplete\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Activity percent complete\"\n    },\n    \"PercentCompleteType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Physical\", \"Duration\", \"Units\"],\n      \"description\": \"Method for calculating percent complete\"\n    },\n    \"PlannedStartDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"PlannedFinishDate\": {\n\
  \      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"ActualStartDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\"\n    },\n    \"ActualFinishDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\"\n    },\n    \"RemainingStartDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\"\n    },\n    \"RemainingFinishDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\"\n    },\n    \"PlannedDuration\": {\n      \"type\": \"number\",\n      \"description\": \"Planned duration in hours\"\n    },\n    \"ActualDuration\": {\n      \"type\": \"number\",\n      \"description\": \"Actual duration accrued in hours\"\n    },\n    \"RemainingDuration\": {\n      \"type\": \"number\",\n      \"description\": \"Remaining duration in hours\"\n    },\n    \"TotalFloat\": {\n      \"type\": \"number\",\n      \"description\": \"Total float in hours; negative values\
  \ indicate critical path\"\n    },\n    \"FreeFloat\": {\n      \"type\": \"number\",\n      \"description\": \"Free float in hours\"\n    },\n    \"CriticalFlag\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if activity is on the critical path\"\n    },\n    \"CalendarObjectId\": {\n      \"type\": \"integer\",\n      \"description\": \"Assigned work calendar ObjectId\"\n    },\n    \"PrimaryConstraintType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"None\",\n        \"Start On\",\n        \"Start On or Before\",\n        \"Start On or After\",\n        \"Finish On\",\n        \"Finish On or Before\",\n        \"Finish On or After\",\n        \"Mandatory Start\",\n        \"Mandatory Finish\",\n        \"As Late as Possible\"\n      ]\n    },\n    \"PrimaryConstraintDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"ObjectId\", \"Id\", \"Name\", \"ProjectObjectId\", \"WBSObjectId\"\
  , \"Type\", \"Status\"],\n  \"examples\": [\n    {\n      \"ObjectId\": 30001,\n      \"Id\": \"A1000\",\n      \"Name\": \"Site Preparation\",\n      \"ProjectObjectId\": 10001,\n      \"WBSObjectId\": 20010,\n      \"Type\": \"Task Dependent\",\n      \"Status\": \"Completed\",\n      \"PercentComplete\": 100.0,\n      \"PercentCompleteType\": \"Physical\",\n      \"PlannedStartDate\": \"2025-01-15T08:00:00Z\",\n      \"PlannedFinishDate\": \"2025-03-01T17:00:00Z\",\n      \"ActualStartDate\": \"2025-01-16T08:00:00Z\",\n      \"ActualFinishDate\": \"2025-03-05T17:00:00Z\",\n      \"PlannedDuration\": 288.0,\n      \"ActualDuration\": 296.0,\n      \"RemainingDuration\": 0.0,\n      \"TotalFloat\": -8.0,\n      \"CriticalFlag\": true\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-primavera/refs/heads/main/json-schema/oracle-primavera-activity-schema.json
tags:
- Construction
- Engineering
- Project Management
- Scheduling
- Portfolio Management
- Oracle
title: Oracle Primavera P6 Activity
---
