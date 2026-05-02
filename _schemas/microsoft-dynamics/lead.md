---
description: A lead in Microsoft Dynamics 365 CRM, representing a potential customer who has not yet been qualified.
layout: schema
name: Lead
properties_list:
- description: The unique identifier of the lead.
  name: leadid
  type: string
- description: The subject or topic of the lead.
  name: subject
  type: string
- description: The first name of the lead.
  name: firstname
  type: string
- description: The last name of the lead.
  name: lastname
  type: string
- description: The full name of the lead.
  name: fullname
  type: string
- description: The company name of the lead.
  name: companyname
  type: string
- description: The job title of the lead.
  name: jobtitle
  type: string
- description: The primary email address.
  name: emailaddress1
  type: string
- description: The primary telephone number.
  name: telephone1
  type: string
- description: The first line of the address.
  name: address1_line1
  type: string
- description: The city of the address.
  name: address1_city
  type: string
- description: The state or province of the address.
  name: address1_stateorprovince
  type: string
- description: The postal code of the address.
  name: address1_postalcode
  type: string
- description: The country of the address.
  name: address1_country
  type: string
- description: The source code indicating where the lead originated.
  name: leadsourcecode
  type: integer
- description: The estimated value of the lead.
  name: estimatedvalue
  type: number
- description: The estimated close date.
  name: estimatedclosedate
  type: string
- description: The state of the lead (0 = Open, 1 = Qualified, 2 = Disqualified).
  name: statecode
  type: integer
- description: The status reason code.
  name: statuscode
  type: integer
- description: The date and time the lead was created.
  name: createdon
  type: string
- description: The date and time the lead was last modified.
  name: modifiedon
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/lead.json
slug: lead
source_filename: lead.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/lead.json\",\n  \"title\": \"Lead\",\n  \"description\": \"A lead in Microsoft Dynamics 365 CRM, representing a potential customer who has not yet been qualified.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"leadid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the lead.\",\n      \"readOnly\": true\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"The subject or topic of the lead.\"\n    },\n    \"firstname\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the lead.\"\n    },\n    \"lastname\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the lead.\"\n    },\n    \"fullname\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The full name of the lead.\",\n      \"readOnly\": true\n    },\n    \"companyname\": {\n      \"type\": \"string\",\n      \"description\": \"The company name of the lead.\"\n    },\n    \"jobtitle\": {\n      \"type\": \"string\",\n      \"description\": \"The job title of the lead.\"\n    },\n    \"emailaddress1\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The primary email address.\"\n    },\n    \"telephone1\": {\n      \"type\": \"string\",\n      \"description\": \"The primary telephone number.\"\n    },\n    \"address1_line1\": {\n      \"type\": \"string\",\n      \"description\": \"The first line of the address.\"\n    },\n    \"address1_city\": {\n      \"type\": \"string\",\n      \"description\": \"The city of the address.\"\n    },\n    \"address1_stateorprovince\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province of the address.\"\n    },\n    \"address1_postalcode\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The postal code of the address.\"\n    },\n    \"address1_country\": {\n      \"type\": \"string\",\n      \"description\": \"The country of the address.\"\n    },\n    \"leadsourcecode\": {\n      \"type\": \"integer\",\n      \"description\": \"The source code indicating where the lead originated.\"\n    },\n    \"estimatedvalue\": {\n      \"type\": \"number\",\n      \"description\": \"The estimated value of the lead.\"\n    },\n    \"estimatedclosedate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The estimated close date.\"\n    },\n    \"statecode\": {\n      \"type\": \"integer\",\n      \"description\": \"The state of the lead (0 = Open, 1 = Qualified, 2 = Disqualified).\"\n    },\n    \"statuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"The status reason code.\"\n    },\n    \"createdon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date\
  \ and time the lead was created.\",\n      \"readOnly\": true\n    },\n    \"modifiedon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the lead was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"lastname\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/lead.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Lead
---
