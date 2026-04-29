---
description: PeopleSoft HCM employee personal data record.
layout: schema
name: Employee
properties_list:
- description: Employee ID.
  name: EMPLID
  type: string
- description: Employee full name.
  name: NAME
  type: string
- description: First name.
  name: FIRST_NAME
  type: string
- description: Last name.
  name: LAST_NAME
  type: string
- description: Department ID.
  name: DEPTID
  type: string
- description: Job code.
  name: JOBCODE
  type: string
- description: Position number.
  name: POSITION_NBR
  type: string
- description: Work location code.
  name: LOCATION
  type: string
- description: Company code.
  name: COMPANY
  type: string
- description: Business unit.
  name: BUSINESS_UNIT
  type: string
- description: Employment status.
  name: EMPL_STATUS
  type: string
- description: HR status.
  name: HR_STATUS
  type: string
- description: Regular or temporary.
  name: REG_TEMP
  type: string
- description: Full or part time.
  name: FULL_PART_TIME
  type: string
- description: Hire date.
  name: HIRE_DT
  type: string
- description: Termination date.
  name: TERMINATION_DT
  type: string
- description: Annual salary rate.
  name: ANNUAL_RT
  type: number
- description: Currency code.
  name: CURRENCY_CD
  type: string
- description: Email address.
  name: EMAIL_ADDR
  type: string
- description: Phone number.
  name: PHONE
  type: string
- description: Street address.
  name: ADDRESS1
  type: string
- description: City.
  name: CITY
  type: string
- description: State code.
  name: STATE
  type: string
- description: Postal code.
  name: POSTAL
  type: string
- description: Country code.
  name: COUNTRY
  type: string
- description: Supervisor employee ID.
  name: SUPERVISOR_ID
  type: string
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-hcm-employee-schema.json
slug: peoplesoft-hcm-employee
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-hcm-employee-schema.json\",\n  \"title\": \"Employee\",\n  \"description\": \"PeopleSoft HCM employee personal data record.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EMPLID\": {\n      \"type\": \"string\",\n      \"description\": \"Employee ID.\",\n      \"example\": \"EMP001234\"\n    },\n    \"NAME\": {\n      \"type\": \"string\",\n      \"description\": \"Employee full name.\",\n      \"example\": \"Jane Smith\"\n    },\n    \"FIRST_NAME\": {\n      \"type\": \"string\",\n      \"description\": \"First name.\",\n      \"example\": \"Jane\"\n    },\n    \"LAST_NAME\": {\n      \"type\": \"string\",\n      \"description\": \"Last name.\",\n      \"example\": \"Smith\"\n    },\n    \"DEPTID\": {\n      \"type\": \"string\",\n      \"description\": \"Department ID.\",\n      \"example\"\
  : \"10200\"\n    },\n    \"JOBCODE\": {\n      \"type\": \"string\",\n      \"description\": \"Job code.\",\n      \"example\": \"MGR001\"\n    },\n    \"POSITION_NBR\": {\n      \"type\": \"string\",\n      \"description\": \"Position number.\",\n      \"example\": \"00012345\"\n    },\n    \"LOCATION\": {\n      \"type\": \"string\",\n      \"description\": \"Work location code.\",\n      \"example\": \"HQ001\"\n    },\n    \"COMPANY\": {\n      \"type\": \"string\",\n      \"description\": \"Company code.\",\n      \"example\": \"CCB\"\n    },\n    \"BUSINESS_UNIT\": {\n      \"type\": \"string\",\n      \"description\": \"Business unit.\",\n      \"example\": \"US001\"\n    },\n    \"EMPL_STATUS\": {\n      \"type\": \"string\",\n      \"description\": \"Employment status.\",\n      \"enum\": [\n        \"A\",\n        \"D\",\n        \"L\",\n        \"P\",\n        \"R\",\n        \"S\",\n        \"T\",\n        \"U\",\n        \"W\",\n        \"X\"\n      ],\n      \"example\": \"\
  A\"\n    },\n    \"HR_STATUS\": {\n      \"type\": \"string\",\n      \"description\": \"HR status.\",\n      \"enum\": [\n        \"A\",\n        \"I\",\n        \"D\"\n      ],\n      \"example\": \"A\"\n    },\n    \"REG_TEMP\": {\n      \"type\": \"string\",\n      \"description\": \"Regular or temporary.\",\n      \"enum\": [\n        \"R\",\n        \"T\"\n      ],\n      \"example\": \"R\"\n    },\n    \"FULL_PART_TIME\": {\n      \"type\": \"string\",\n      \"description\": \"Full or part time.\",\n      \"enum\": [\n        \"F\",\n        \"P\"\n      ],\n      \"example\": \"F\"\n    },\n    \"HIRE_DT\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Hire date.\",\n      \"example\": \"2020-01-15\"\n    },\n    \"TERMINATION_DT\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Termination date.\"\n    },\n    \"ANNUAL_RT\": {\n      \"type\": \"number\",\n      \"description\": \"Annual salary rate.\"\
  ,\n      \"example\": 85000.0\n    },\n    \"CURRENCY_CD\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code.\",\n      \"example\": \"USD\"\n    },\n    \"EMAIL_ADDR\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address.\",\n      \"example\": \"jane.smith@example.com\"\n    },\n    \"PHONE\": {\n      \"type\": \"string\",\n      \"description\": \"Phone number.\",\n      \"example\": \"555-0123\"\n    },\n    \"ADDRESS1\": {\n      \"type\": \"string\",\n      \"description\": \"Street address.\",\n      \"example\": \"123 Main St\"\n    },\n    \"CITY\": {\n      \"type\": \"string\",\n      \"description\": \"City.\",\n      \"example\": \"San Francisco\"\n    },\n    \"STATE\": {\n      \"type\": \"string\",\n      \"description\": \"State code.\",\n      \"example\": \"CA\"\n    },\n    \"POSTAL\": {\n      \"type\": \"string\",\n      \"description\": \"Postal code.\",\n      \"example\": \"94105\"\n    },\n\
  \    \"COUNTRY\": {\n      \"type\": \"string\",\n      \"description\": \"Country code.\",\n      \"example\": \"USA\"\n    },\n    \"SUPERVISOR_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Supervisor employee ID.\",\n      \"example\": \"EMP000567\"\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-hcm-employee-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: Employee
---
