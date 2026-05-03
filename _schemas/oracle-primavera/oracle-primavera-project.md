---
description: Schema for an Oracle Primavera P6 EPPM project, representing an enterprise project with schedule, cost, and resource data.
layout: schema
name: Oracle Primavera P6 Project
properties_list:
- description: System-generated unique identifier
  name: ObjectId
  type: integer
- description: User-defined project ID
  name: Id
  type: string
- description: Project name
  name: Name
  type: string
- description: Current project status
  name: Status
  type: string
- description: Planned project start date
  name: PlannedStartDate
  type: string
- description: Planned project finish date
  name: PlannedFinishDate
  type: string
- description: Actual project start date
  name: ActualStartDate
  type:
  - string
  - 'null'
- description: Actual project finish date
  name: ActualFinishDate
  type:
  - string
  - 'null'
- description: Status date used for progress tracking
  name: DataDate
  type: string
- description: Overall project percent complete
  name: PercentComplete
  type: number
- description: Total budget at completion cost
  name: TotalBudgetCost
  type: number
- description: Actual total cost to date
  name: ActualTotalCost
  type: number
- description: Budgeted cost of work performed (BCWP)
  name: EarnedValueCost
  type: number
- description: Budgeted cost of work scheduled (BCWS)
  name: PlannedValueCost
  type: number
- description: Earned value CPI (BCWP / ACWP)
  name: CostPerformanceIndex
  type: number
- description: Earned value SPI (BCWP / BCWS)
  name: SchedulePerformanceIndex
  type: number
- description: Project risk rating
  name: RiskLevel
  type: string
- description: Root WBS element ObjectId
  name: WBSObjectId
  type: integer
- description: Responsible OBS node ObjectId
  name: OBSObjectId
  type: integer
- description: Date the project was created
  name: CreateDate
  type: string
- description: Date the project was last modified
  name: LastUpdateDate
  type: string
provider_name: Oracle Primavera
provider_slug: oracle-primavera
schema_file: json-schema/oracle-primavera-project-schema.json
slug: oracle-primavera-project
source_filename: oracle-primavera-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/oracle-primavera/json-schema/oracle-primavera-project-schema.json\",\n  \"title\": \"Oracle Primavera P6 Project\",\n  \"description\": \"Schema for an Oracle Primavera P6 EPPM project, representing an enterprise project with schedule, cost, and resource data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ObjectId\": {\n      \"type\": \"integer\",\n      \"description\": \"System-generated unique identifier\"\n    },\n    \"Id\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"User-defined project ID\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"Project name\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\", \"What-if\", \"Planned\"],\n      \"description\": \"Current project status\"\n    },\n    \"PlannedStartDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Planned project start date\"\n    },\n    \"PlannedFinishDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Planned project finish date\"\n    },\n    \"ActualStartDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Actual project start date\"\n    },\n    \"ActualFinishDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"Actual project finish date\"\n    },\n    \"DataDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Status date used for progress tracking\"\n    },\n    \"PercentComplete\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Overall project percent complete\"\n    },\n    \"TotalBudgetCost\": {\n      \"type\": \"\
  number\",\n      \"description\": \"Total budget at completion cost\"\n    },\n    \"ActualTotalCost\": {\n      \"type\": \"number\",\n      \"description\": \"Actual total cost to date\"\n    },\n    \"EarnedValueCost\": {\n      \"type\": \"number\",\n      \"description\": \"Budgeted cost of work performed (BCWP)\"\n    },\n    \"PlannedValueCost\": {\n      \"type\": \"number\",\n      \"description\": \"Budgeted cost of work scheduled (BCWS)\"\n    },\n    \"CostPerformanceIndex\": {\n      \"type\": \"number\",\n      \"description\": \"Earned value CPI (BCWP / ACWP)\"\n    },\n    \"SchedulePerformanceIndex\": {\n      \"type\": \"number\",\n      \"description\": \"Earned value SPI (BCWP / BCWS)\"\n    },\n    \"RiskLevel\": {\n      \"type\": \"string\",\n      \"enum\": [\"Very High\", \"High\", \"Medium\", \"Low\", \"Very Low\"],\n      \"description\": \"Project risk rating\"\n    },\n    \"WBSObjectId\": {\n      \"type\": \"integer\",\n      \"description\": \"Root WBS element\
  \ ObjectId\"\n    },\n    \"OBSObjectId\": {\n      \"type\": \"integer\",\n      \"description\": \"Responsible OBS node ObjectId\"\n    },\n    \"CreateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the project was created\"\n    },\n    \"LastUpdateDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Date the project was last modified\"\n    }\n  },\n  \"required\": [\"ObjectId\", \"Id\", \"Name\", \"Status\"],\n  \"examples\": [\n    {\n      \"ObjectId\": 10001,\n      \"Id\": \"PROJ-001\",\n      \"Name\": \"North Terminal Expansion\",\n      \"Status\": \"Active\",\n      \"PlannedStartDate\": \"2025-01-15T00:00:00Z\",\n      \"PlannedFinishDate\": \"2026-12-31T00:00:00Z\",\n      \"DataDate\": \"2026-03-01T00:00:00Z\",\n      \"PercentComplete\": 28.5,\n      \"TotalBudgetCost\": 45000000.0,\n      \"EarnedValueCost\": 12825000.0,\n      \"RiskLevel\": \"Medium\",\n      \"WBSObjectId\"\
  : 20001\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-primavera/refs/heads/main/json-schema/oracle-primavera-project-schema.json
tags:
- Construction
- Engineering
- Project Management
- Scheduling
- Portfolio Management
- Oracle
title: Oracle Primavera P6 Project
---
