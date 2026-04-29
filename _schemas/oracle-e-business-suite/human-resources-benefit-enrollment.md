---
description: ''
layout: schema
name: BenefitEnrollment
properties_list:
- description: Enrollment result identifier
  name: enrollmentResultId
  type: integer
- description: Person identifier
  name: personId
  type: integer
- description: Benefit plan identifier
  name: planId
  type: integer
- description: Plan name
  name: planName
  type: string
- description: Option identifier
  name: optionId
  type: integer
- description: Option name
  name: optionName
  type: string
- description: Coverage level
  name: coverageLevelCode
  type: string
- description: ''
  name: effectiveStartDate
  type: string
- description: ''
  name: effectiveEndDate
  type: string
- description: ''
  name: enrollmentStartDate
  type: string
- description: ''
  name: enrollmentEndDate
  type: string
- description: Benefit coverage amount
  name: benefitAmount
  type: number
provider_name: Oracle E-Business Suite
provider_slug: oracle-e-business-suite
schema_file: json-schema/human-resources-benefit-enrollment-schema.json
slug: human-resources-benefit-enrollment
source_filename: human-resources-benefit-enrollment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BenefitEnrollment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"enrollmentResultId\": {\n      \"type\": \"integer\",\n      \"description\": \"Enrollment result identifier\"\n    },\n    \"personId\": {\n      \"type\": \"integer\",\n      \"description\": \"Person identifier\"\n    },\n    \"planId\": {\n      \"type\": \"integer\",\n      \"description\": \"Benefit plan identifier\"\n    },\n    \"planName\": {\n      \"type\": \"string\",\n      \"description\": \"Plan name\"\n    },\n    \"optionId\": {\n      \"type\": \"integer\",\n      \"description\": \"Option identifier\"\n    },\n    \"optionName\": {\n      \"type\": \"string\",\n      \"description\": \"Option name\"\n    },\n    \"coverageLevelCode\": {\n      \"type\": \"string\",\n      \"description\": \"Coverage level\"\n    },\n    \"effectiveStartDate\": {\n      \"type\": \"string\"\n    },\n    \"effectiveEndDate\"\
  : {\n      \"type\": \"string\"\n    },\n    \"enrollmentStartDate\": {\n      \"type\": \"string\"\n    },\n    \"enrollmentEndDate\": {\n      \"type\": \"string\"\n    },\n    \"benefitAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Benefit coverage amount\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-e-business-suite/refs/heads/main/json-schema/human-resources-benefit-enrollment-schema.json
tags:
- Business Applications
- E-Business Suite
- Enterprise
- ERP
- Oracle
title: BenefitEnrollment
---
