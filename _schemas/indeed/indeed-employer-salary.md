---
description: Salary or compensation details for the job posting.
layout: schema
name: Salary
properties_list:
- description: The minimum salary amount.
  name: minimumAmount
  type: number
- description: The maximum salary amount.
  name: maximumAmount
  type: number
- description: ISO 4217 currency code.
  name: currency
  type: string
- description: The pay period for the salary.
  name: period
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-salary-schema.json
slug: indeed-employer-salary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Salary\",\n  \"type\": \"object\",\n  \"description\": \"Salary or compensation details for the job posting.\",\n  \"properties\": {\n    \"minimumAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum salary amount.\"\n    },\n    \"maximumAmount\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum salary amount.\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code.\"\n    },\n    \"period\": {\n      \"type\": \"string\",\n      \"description\": \"The pay period for the salary.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-salary-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: Salary
---
