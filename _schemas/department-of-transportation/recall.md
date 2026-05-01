---
description: A vehicle, equipment, child-seat, or tire recall record published by NHTSA.
layout: schema
name: NHTSA Vehicle Recall
properties_list:
- description: NHTSA recall campaign identifier
  name: NHTSACampaignNumber
  type: string
- description: ''
  name: Manufacturer
  type: string
- description: ''
  name: ReportReceivedDate
  type: string
- description: ''
  name: Component
  type: string
- description: ''
  name: Summary
  type: string
- description: ''
  name: Consequence
  type: string
- description: ''
  name: Remedy
  type: string
- description: ''
  name: Notes
  type:
  - string
  - 'null'
- description: ''
  name: ModelYear
  type: string
- description: ''
  name: Make
  type: string
- description: ''
  name: Model
  type: string
- description: ''
  name: PotentialNumberOfUnitsAffected
  type:
  - string
  - integer
provider_name: Department of Transportation
provider_slug: department-of-transportation
schema_file: json-schema/recall-schema.json
slug: recall
source_filename: recall-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-transportation/schemas/recall.json\",\n  \"title\": \"NHTSA Vehicle Recall\",\n  \"description\": \"A vehicle, equipment, child-seat, or tire recall record published by NHTSA.\",\n  \"type\": \"object\",\n  \"required\": [\"NHTSACampaignNumber\", \"Manufacturer\"],\n  \"properties\": {\n    \"NHTSACampaignNumber\": { \"type\": \"string\", \"description\": \"NHTSA recall campaign identifier\" },\n    \"Manufacturer\": { \"type\": \"string\" },\n    \"ReportReceivedDate\": { \"type\": \"string\" },\n    \"Component\": { \"type\": \"string\" },\n    \"Summary\": { \"type\": \"string\" },\n    \"Consequence\": { \"type\": \"string\" },\n    \"Remedy\": { \"type\": \"string\" },\n    \"Notes\": { \"type\": [\"string\", \"null\"] },\n    \"ModelYear\": { \"type\": \"string\" },\n    \"Make\": { \"type\": \"string\" },\n    \"Model\": { \"type\": \"string\" },\n\
  \    \"PotentialNumberOfUnitsAffected\": { \"type\": [\"string\", \"integer\"] }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-transportation/refs/heads/main/json-schema/recall-schema.json
tags:
- Federal Government
- Transportation
- Vehicles
- Aviation
- Motor Carriers
title: NHTSA Vehicle Recall
---
