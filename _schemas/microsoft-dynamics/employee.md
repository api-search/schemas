---
description: An employee record in Microsoft Dynamics 365 Business Central.
layout: schema
name: Employee
properties_list:
- description: The unique identifier of the employee.
  name: id
  type: string
- description: The employee number.
  name: number
  type: string
- description: The display name of the employee.
  name: displayName
  type: string
- description: The given (first) name.
  name: givenName
  type: string
- description: The middle name.
  name: middleName
  type: string
- description: The surname (last name).
  name: surname
  type: string
- description: The job title of the employee.
  name: jobTitle
  type: string
- description: The first line of the employee address.
  name: addressLine1
  type: string
- description: The second line of the employee address.
  name: addressLine2
  type: string
- description: The city of the employee address.
  name: city
  type: string
- description: The state or province of the employee address.
  name: state
  type: string
- description: The country of the employee address.
  name: country
  type: string
- description: The postal code of the employee address.
  name: postalCode
  type: string
- description: The phone number.
  name: phoneNumber
  type: string
- description: The mobile phone number.
  name: mobilePhone
  type: string
- description: The work email address.
  name: email
  type: string
- description: The personal email address.
  name: personalEmail
  type: string
- description: The employment start date.
  name: employmentDate
  type: string
- description: The termination date.
  name: terminationDate
  type: string
- description: The employment status.
  name: status
  type: string
- description: The date of birth.
  name: birthDate
  type: string
- description: The date and time the record was last modified.
  name: lastModifiedDateTime
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/employee.json
slug: employee
source_filename: employee.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/employee.json\",\n  \"title\": \"Employee\",\n  \"description\": \"An employee record in Microsoft Dynamics 365 Business Central.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the employee.\",\n      \"readOnly\": true\n    },\n    \"number\": {\n      \"type\": \"string\",\n      \"description\": \"The employee number.\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the employee.\"\n    },\n    \"givenName\": {\n      \"type\": \"string\",\n      \"description\": \"The given (first) name.\"\n    },\n    \"middleName\": {\n      \"type\": \"string\",\n      \"description\": \"The middle name.\"\n    },\n    \"surname\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The surname (last name).\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"description\": \"The job title of the employee.\"\n    },\n    \"addressLine1\": {\n      \"type\": \"string\",\n      \"description\": \"The first line of the employee address.\"\n    },\n    \"addressLine2\": {\n      \"type\": \"string\",\n      \"description\": \"The second line of the employee address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"The city of the employee address.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province of the employee address.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country of the employee address.\"\n    },\n    \"postalCode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the employee address.\"\n    },\n    \"phoneNumber\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"The phone number.\"\n    },\n    \"mobilePhone\": {\n      \"type\": \"string\",\n      \"description\": \"The mobile phone number.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The work email address.\"\n    },\n    \"personalEmail\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The personal email address.\"\n    },\n    \"employmentDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The employment start date.\"\n    },\n    \"terminationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The termination date.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Inactive\"],\n      \"description\": \"The employment status.\"\n    },\n    \"birthDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\
  ,\n      \"description\": \"The date of birth.\"\n    },\n    \"lastModifiedDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the record was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/employee.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Employee
---
