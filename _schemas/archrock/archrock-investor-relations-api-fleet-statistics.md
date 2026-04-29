---
description: ''
layout: schema
name: FleetStatistics
properties_list:
- description: ''
  name: year
  type: integer
- description: ''
  name: quarter
  type: integer
- description: Total fleet horsepower
  name: totalHorsepower
  type: integer
- description: Active fleet horsepower
  name: activeHorsepower
  type: integer
- description: Fleet utilization rate as percentage
  name: utilizationRate
  type: number
- description: ''
  name: averageHorsepowerPerUnit
  type: number
- description: ''
  name: totalUnits
  type: integer
- description: ''
  name: newUnitDeployments
  type: integer
- description: ''
  name: unitRetirements
  type: integer
provider_name: Archrock
provider_slug: archrock
schema_file: json-schema/archrock-investor-relations-api-fleet-statistics-schema.json
slug: archrock-investor-relations-api-fleet-statistics
source_filename: archrock-investor-relations-api-fleet-statistics-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-fleet-statistics-schema.json\",\n  \"title\": \"FleetStatistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"year\": {\n      \"type\": \"integer\"\n    },\n    \"quarter\": {\n      \"type\": \"integer\"\n    },\n    \"totalHorsepower\": {\n      \"type\": \"integer\",\n      \"description\": \"Total fleet horsepower\"\n    },\n    \"activeHorsepower\": {\n      \"type\": \"integer\",\n      \"description\": \"Active fleet horsepower\"\n    },\n    \"utilizationRate\": {\n      \"type\": \"number\",\n      \"description\": \"Fleet utilization rate as percentage\"\n    },\n    \"averageHorsepowerPerUnit\": {\n      \"type\": \"number\"\n    },\n    \"totalUnits\": {\n      \"type\": \"integer\"\n    },\n    \"newUnitDeployments\": {\n      \"type\": \"integer\"\n   \
  \ },\n    \"unitRetirements\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/archrock/refs/heads/main/json-schema/archrock-investor-relations-api-fleet-statistics-schema.json
tags:
- Natural Gas
- Compression Services
- Oil And Gas
- Energy
- Industrial
- 'NYSE: AROC'
title: FleetStatistics
---
