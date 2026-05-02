---
description: An account in Microsoft Dynamics 365 CRM, representing a business organization such as a customer, competitor, or partner.
layout: schema
name: Account
properties_list:
- description: The unique identifier of the account.
  name: accountid
  type: string
- description: The name of the account.
  name: name
  type: string
- description: The account number.
  name: accountnumber
  type: string
- description: Additional information about the account.
  name: description
  type: string
- description: The annual revenue of the account.
  name: revenue
  type: number
- description: The number of employees at the account.
  name: numberofemployees
  type: integer
- description: The industry classification code.
  name: industrycode
  type: integer
- description: The first line of the primary address.
  name: address1_line1
  type: string
- description: The city of the primary address.
  name: address1_city
  type: string
- description: The state or province of the primary address.
  name: address1_stateorprovince
  type: string
- description: The postal code of the primary address.
  name: address1_postalcode
  type: string
- description: The country of the primary address.
  name: address1_country
  type: string
- description: The primary telephone number.
  name: telephone1
  type: string
- description: The primary email address.
  name: emailaddress1
  type: string
- description: The website URL.
  name: websiteurl
  type: string
- description: The state of the account (0 = Active, 1 = Inactive).
  name: statecode
  type: integer
- description: The status reason code.
  name: statuscode
  type: integer
- description: The date and time the account was created.
  name: createdon
  type: string
- description: The date and time the account was last modified.
  name: modifiedon
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/account.json
slug: account
source_filename: account.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/account.json\",\n  \"title\": \"Account\",\n  \"description\": \"An account in Microsoft Dynamics 365 CRM, representing a business organization such as a customer, competitor, or partner.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the account.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the account.\"\n    },\n    \"accountnumber\": {\n      \"type\": \"string\",\n      \"description\": \"The account number.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional information about the account.\"\n    },\n    \"revenue\": {\n      \"type\": \"number\"\
  ,\n      \"description\": \"The annual revenue of the account.\"\n    },\n    \"numberofemployees\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of employees at the account.\"\n    },\n    \"industrycode\": {\n      \"type\": \"integer\",\n      \"description\": \"The industry classification code.\"\n    },\n    \"address1_line1\": {\n      \"type\": \"string\",\n      \"description\": \"The first line of the primary address.\"\n    },\n    \"address1_city\": {\n      \"type\": \"string\",\n      \"description\": \"The city of the primary address.\"\n    },\n    \"address1_stateorprovince\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province of the primary address.\"\n    },\n    \"address1_postalcode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the primary address.\"\n    },\n    \"address1_country\": {\n      \"type\": \"string\",\n      \"description\": \"The country of the primary address.\"\n  \
  \  },\n    \"telephone1\": {\n      \"type\": \"string\",\n      \"description\": \"The primary telephone number.\"\n    },\n    \"emailaddress1\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The primary email address.\"\n    },\n    \"websiteurl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The website URL.\"\n    },\n    \"statecode\": {\n      \"type\": \"integer\",\n      \"description\": \"The state of the account (0 = Active, 1 = Inactive).\"\n    },\n    \"statuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"The status reason code.\"\n    },\n    \"createdon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the account was created.\",\n      \"readOnly\": true\n    },\n    \"modifiedon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the account was last\
  \ modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/account.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Account
---
