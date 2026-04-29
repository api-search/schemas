---
description: Mileage-specific data for distance-based expenses
layout: schema
name: Mileage
properties_list:
- description: Total distance traveled
  name: totalDistance
  type: integer
- description: The identifier of the vehicle used
  name: vehicleId
  type: string
- description: Starting odometer reading
  name: odometerStart
  type: integer
- description: Ending odometer reading
  name: odometerEnd
  type: integer
- description: Number of passengers
  name: passengerCount
  type: integer
- description: Distance attributed to personal use
  name: personalDistance
  type: integer
- description: Whether the higher mileage rate applies
  name: isMarkedAsHigherRate
  type: boolean
- description: The identifier of the route taken
  name: routeId
  type: string
- description: Whether equipment was transported
  name: hasMachinery
  type: boolean
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-mileage-schema.json
slug: sap-concur-expense-mileage
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Mileage\",\n  \"type\": \"object\",\n  \"description\": \"Mileage-specific data for distance-based expenses\",\n  \"properties\": {\n    \"totalDistance\": {\n      \"type\": \"integer\",\n      \"description\": \"Total distance traveled\"\n    },\n    \"vehicleId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the vehicle used\"\n    },\n    \"odometerStart\": {\n      \"type\": \"integer\",\n      \"description\": \"Starting odometer reading\"\n    },\n    \"odometerEnd\": {\n      \"type\": \"integer\",\n      \"description\": \"Ending odometer reading\"\n    },\n    \"passengerCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of passengers\"\n    },\n    \"personalDistance\": {\n      \"type\": \"integer\",\n      \"description\": \"Distance attributed to personal use\"\n    },\n    \"isMarkedAsHigherRate\": {\n      \"type\": \"boolean\"\
  ,\n      \"description\": \"Whether the higher mileage rate applies\"\n    },\n    \"routeId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the route taken\"\n    },\n    \"hasMachinery\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether equipment was transported\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-mileage-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Mileage
---
