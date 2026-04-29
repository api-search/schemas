---
description: Travel-specific data for transportation expenses
layout: schema
name: Travel
properties_list:
- description: Trip origin location
  name: startLocation
  type: string
- description: Trip destination location
  name: endLocation
  type: string
- description: Ticket or booking reference number
  name: ticketNumber
  type: string
- description: Hotel check-in date
  name: hotelCheckinDate
  type: string
- description: Hotel check-out date
  name: hotelCheckoutDate
  type: string
- description: Number of car rental days
  name: carRentalDays
  type: integer
- description: Airline cabin class code
  name: airlineServiceClassCode
  type: string
- description: Airline fee type identifier
  name: airlineFeeTypeCode
  type: string
provider_name: SAP Concur
provider_slug: sap-concur
schema_file: json-schema/sap-concur-expense-travel-schema.json
slug: sap-concur-expense-travel
source_filename: sap-concur-expense-travel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Travel\",\n  \"type\": \"object\",\n  \"description\": \"Travel-specific data for transportation expenses\",\n  \"properties\": {\n    \"startLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Trip origin location\"\n    },\n    \"endLocation\": {\n      \"type\": \"string\",\n      \"description\": \"Trip destination location\"\n    },\n    \"ticketNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Ticket or booking reference number\"\n    },\n    \"hotelCheckinDate\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel check-in date\"\n    },\n    \"hotelCheckoutDate\": {\n      \"type\": \"string\",\n      \"description\": \"Hotel check-out date\"\n    },\n    \"carRentalDays\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of car rental days\"\n    },\n    \"airlineServiceClassCode\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Airline cabin class code\"\n    },\n    \"airlineFeeTypeCode\": {\n      \"type\": \"string\",\n      \"description\": \"Airline fee type identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-concur/refs/heads/main/json-schema/sap-concur-expense-travel-schema.json
tags:
- Business Travel
- Expense Management
- Financial Services
- Invoice Management
- Travel Management
title: Travel
---
