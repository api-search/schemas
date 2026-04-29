---
description: List of executives and their compensation details for the specified company identifier.
layout: schema
name: companyCompensation
properties_list:
- description: FactSet Name of the person
  name: name
  type: string
- description: Factset Entity Identifier for the Person
  name: personId
  type: string
- description: The requested Position Title
  name: title
  type: string
- description: Salary of the person. Expressed in USD and raw units.
  name: salary
  type: number
- description: Bonus of the executive during the fiscal year. Expressed in USD and raw units.
  name: bonus
  type: number
- description: Stock awards for the person. Expressed in USD and raw units.
  name: stockAwards
  type: number
- description: Option Awards for the person. Expressed in USD and raw units.
  name: optionsAwards
  type: number
- description: All the other compensations which are not explicitly defined as salary, bonus, stock awards, or options awards. Expressed in USD and raw units.
  name: otherCompensation
  type: number
- description: The sum of all compensation for the requested person as reported by the company. Expressed in USD and raw units.
  name: totalCompensation
  type: number
- description: All the earnings pursuant to awards under non-equity incentive plans. Expressed in USD and raw units.
  name: nonEquityIncentivePlanComp
  type: number
- description: All the other nonqualified defined contribution which are not tax qualified and other contributions. Expressed in USD and raw units.
  name: nonQualifiedCompEarnings
  type: number
- description: The most recent year of compensation is expressed as 'YYYY' as opposed to 'YYYY-MM-DD' format.
  name: compensationYear
  type: string
- description: Original identifier used for the request.
  name: requestId
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-people-company-compensation-schema.json
slug: factset-people-company-compensation
source_filename: factset-people-company-compensation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"companyCompensation\",\n  \"type\": \"object\",\n  \"description\": \"List of executives and their compensation details for the specified company identifier.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Name of the person\"\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"Factset Entity Identifier for the Person\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The requested Position Title\"\n    },\n    \"salary\": {\n      \"type\": \"number\",\n      \"description\": \"Salary of the person. Expressed in USD and raw units.\"\n    },\n    \"bonus\": {\n      \"type\": \"number\",\n      \"description\": \"Bonus of the executive during the fiscal year. Expressed in USD and raw units.\"\n    },\n    \"stockAwards\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Stock awards for the person. Expressed in USD and raw units.\"\n    },\n    \"optionsAwards\": {\n      \"type\": \"number\",\n      \"description\": \"Option Awards for the person. Expressed in USD and raw units.\"\n    },\n    \"otherCompensation\": {\n      \"type\": \"number\",\n      \"description\": \"All the other compensations which are not explicitly defined as salary, bonus, stock awards, or options awards. Expressed in USD and raw units.\"\n    },\n    \"totalCompensation\": {\n      \"type\": \"number\",\n      \"description\": \"The sum of all compensation for the requested person as reported by the company. Expressed in USD and raw units.\"\n    },\n    \"nonEquityIncentivePlanComp\": {\n      \"type\": \"number\",\n      \"description\": \"All the earnings pursuant to awards under non-equity incentive plans. Expressed in USD and raw units.\"\n    },\n    \"nonQualifiedCompEarnings\": {\n      \"type\": \"number\",\n      \"description\": \"All the other nonqualified\
  \ defined contribution which are not tax qualified and other contributions. Expressed in USD and raw units.\"\n    },\n    \"compensationYear\": {\n      \"type\": \"string\",\n      \"description\": \"The most recent year of compensation is expressed as 'YYYY' as opposed to 'YYYY-MM-DD' format.\"\n    },\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Original identifier used for the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-people-company-compensation-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: companyCompensation
---
