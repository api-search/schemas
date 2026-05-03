---
description: Schema for a sustainability goal or net zero commitment in Salesforce Net Zero Cloud.
layout: schema
name: Salesforce Net Zero Cloud Sustainability Goal
properties_list:
- description: Salesforce record ID
  name: Id
  type: string
- description: Name of the sustainability goal
  name: Name
  type: string
- description: Type of sustainability goal
  name: GoalType
  type: string
- description: The reference year from which reductions are measured
  name: BaselineYear
  type: integer
- description: The year by which the goal should be achieved
  name: TargetYear
  type: integer
- description: Target reduction percentage from baseline
  name: ReductionTargetPercentage
  type: number
- description: Current progress toward the goal as a percentage
  name: CurrentProgressPercentage
  type: number
- description: Current status of the goal
  name: Status
  type: string
- description: Description of the goal and its scope
  name: Description
  type: string
- description: Timestamp when the goal was created
  name: CreatedDate
  type: string
provider_name: Salesforce Net Zero Cloud
provider_slug: salesforce-net-zero-cloud
schema_file: json-schema/salesforce-net-zero-cloud-sustainability-goal-schema.json
slug: salesforce-net-zero-cloud-sustainability-goal
source_filename: salesforce-net-zero-cloud-sustainability-goal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/salesforce-net-zero-cloud/blob/main/json-schema/salesforce-net-zero-cloud-sustainability-goal-schema.json\",\n  \"title\": \"Salesforce Net Zero Cloud Sustainability Goal\",\n  \"description\": \"Schema for a sustainability goal or net zero commitment in Salesforce Net Zero Cloud.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce record ID\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the sustainability goal\"\n    },\n    \"GoalType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of sustainability goal\",\n      \"enum\": [\n        \"NetZero\",\n        \"CarbonNeutral\",\n        \"ScienceBasedTarget\",\n        \"RenewableEnergy\",\n        \"WasteReduction\",\n        \"WaterReduction\"\n      ]\n    },\n    \"BaselineYear\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The reference year from which reductions are measured\",\n      \"minimum\": 1990,\n      \"maximum\": 2100\n    },\n    \"TargetYear\": {\n      \"type\": \"integer\",\n      \"description\": \"The year by which the goal should be achieved\",\n      \"minimum\": 1990,\n      \"maximum\": 2100\n    },\n    \"ReductionTargetPercentage\": {\n      \"type\": \"number\",\n      \"description\": \"Target reduction percentage from baseline\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"CurrentProgressPercentage\": {\n      \"type\": \"number\",\n      \"description\": \"Current progress toward the goal as a percentage\",\n      \"minimum\": 0,\n      \"maximum\": 200\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the goal\",\n      \"enum\": [\"Active\", \"Achieved\", \"Missed\", \"InProgress\"]\n    },\n    \"Description\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Description of the goal and its scope\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the goal was created\"\n    }\n  },\n  \"required\": [\"GoalType\", \"BaselineYear\", \"TargetYear\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce-net-zero-cloud/refs/heads/main/json-schema/salesforce-net-zero-cloud-sustainability-goal-schema.json
tags:
- Carbon Accounting
- Carbon Emissions
- Climate
- Environmental
- ESG
- Net Zero
- Sustainability
title: Salesforce Net Zero Cloud Sustainability Goal
---
