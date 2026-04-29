---
description: Basic information about a person entity.
layout: schema
name: profile
properties_list:
- description: Person identifier used in the request.
  name: requestId
  type: string
- description: FactSet Entity Identifier for the Person
  name: personId
  type: string
- description: Last Name
  name: lastName
  type: string
- description: Name
  name: factsetName
  type: string
- description: First Name
  name: firstName
  type: string
- description: Middle Name
  name: middleName
  type: string
- description: Formal Name
  name: formalName
  type: string
- description: Proper Name
  name: properName
  type: string
- description: Primary Salutation of Name
  name: salutation
  type: string
- description: The Highest Held Degree Code.
  name: highestDegree
  type: string
- description: The Highest Degree Institution Name.
  name: highestDegreeInst
  type: string
- description: Suffix of Name
  name: suffix
  type: string
- description: Person's age in years.
  name: age
  type: number
- description: Person's Gender.
  name: gender
  type: string
- description: Most Recent Salary
  name: salary
  type: number
- description: Most Recent Total Compensation
  name: totalCompensation
  type: number
- description: Entity identifier of primary `Company` of employment.
  name: primaryCompanyId
  type: string
- description: Name of primary company of employment
  name: primaryCompanyName
  type: string
- description: Title at primary `Company` of employment
  name: primaryTitle
  type: string
- description: Brief biography of the person requested.
  name: biography
  type: string
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-people-profile-schema.json
slug: factset-people-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"profile\",\n  \"type\": \"object\",\n  \"description\": \"Basic information about a person entity.\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Person identifier used in the request.\"\n    },\n    \"personId\": {\n      \"type\": \"string\",\n      \"description\": \"FactSet Entity Identifier for the Person\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last Name\"\n    },\n    \"factsetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name\"\n    },\n    \"firstName\": {\n      \"type\": \"string\",\n      \"description\": \"First Name\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"description\": \"Middle Name\"\n    },\n    \"formalName\": {\n      \"type\": \"string\",\n      \"description\": \"Formal Name\"\n    },\n    \"properName\": {\n      \"type\":\
  \ \"string\",\n      \"description\": \"Proper Name\"\n    },\n    \"salutation\": {\n      \"type\": \"string\",\n      \"description\": \"Primary Salutation of Name\"\n    },\n    \"highestDegree\": {\n      \"type\": \"string\",\n      \"description\": \"The Highest Held Degree Code.\"\n    },\n    \"highestDegreeInst\": {\n      \"type\": \"string\",\n      \"description\": \"The Highest Degree Institution Name.\"\n    },\n    \"suffix\": {\n      \"type\": \"string\",\n      \"description\": \"Suffix of Name\"\n    },\n    \"age\": {\n      \"type\": \"number\",\n      \"description\": \"Person's age in years.\"\n    },\n    \"gender\": {\n      \"type\": \"string\",\n      \"description\": \"Person's Gender.\"\n    },\n    \"salary\": {\n      \"type\": \"number\",\n      \"description\": \"Most Recent Salary\"\n    },\n    \"totalCompensation\": {\n      \"type\": \"number\",\n      \"description\": \"Most Recent Total Compensation\"\n    },\n    \"primaryCompanyId\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Entity identifier of primary `Company` of employment.\"\n    },\n    \"primaryCompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of primary company of employment\"\n    },\n    \"primaryTitle\": {\n      \"type\": \"string\",\n      \"description\": \"Title at primary `Company` of employment\"\n    },\n    \"biography\": {\n      \"type\": \"string\",\n      \"description\": \"Brief biography of the person requested.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-people-profile-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: profile
---
