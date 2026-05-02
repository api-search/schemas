---
description: A contact in Microsoft Dynamics 365 CRM, representing an individual person associated with an account.
layout: schema
name: Contact
properties_list:
- description: The unique identifier of the contact.
  name: contactid
  type: string
- description: The first name of the contact.
  name: firstname
  type: string
- description: The last name of the contact.
  name: lastname
  type: string
- description: The full name of the contact.
  name: fullname
  type: string
- description: The job title of the contact.
  name: jobtitle
  type: string
- description: The primary email address.
  name: emailaddress1
  type: string
- description: The primary telephone number.
  name: telephone1
  type: string
- description: The mobile phone number.
  name: mobilephone
  type: string
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
- description: The date of birth of the contact.
  name: birthdate
  type: string
- description: The state of the contact (0 = Active, 1 = Inactive).
  name: statecode
  type: integer
- description: The status reason code.
  name: statuscode
  type: integer
- description: The date and time the contact was created.
  name: createdon
  type: string
- description: The date and time the contact was last modified.
  name: modifiedon
  type: string
provider_name: Microsoft Dynamics
provider_slug: microsoft-dynamics
schema_file: json-schema/contact.json
slug: contact
source_filename: contact.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/contact.json\",\n  \"title\": \"Contact\",\n  \"description\": \"A contact in Microsoft Dynamics 365 CRM, representing an individual person associated with an account.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contactid\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier of the contact.\",\n      \"readOnly\": true\n    },\n    \"firstname\": {\n      \"type\": \"string\",\n      \"description\": \"The first name of the contact.\"\n    },\n    \"lastname\": {\n      \"type\": \"string\",\n      \"description\": \"The last name of the contact.\"\n    },\n    \"fullname\": {\n      \"type\": \"string\",\n      \"description\": \"The full name of the contact.\",\n      \"readOnly\": true\n    },\n    \"jobtitle\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The job title of the contact.\"\n    },\n    \"emailaddress1\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The primary email address.\"\n    },\n    \"telephone1\": {\n      \"type\": \"string\",\n      \"description\": \"The primary telephone number.\"\n    },\n    \"mobilephone\": {\n      \"type\": \"string\",\n      \"description\": \"The mobile phone number.\"\n    },\n    \"address1_line1\": {\n      \"type\": \"string\",\n      \"description\": \"The first line of the primary address.\"\n    },\n    \"address1_city\": {\n      \"type\": \"string\",\n      \"description\": \"The city of the primary address.\"\n    },\n    \"address1_stateorprovince\": {\n      \"type\": \"string\",\n      \"description\": \"The state or province of the primary address.\"\n    },\n    \"address1_postalcode\": {\n      \"type\": \"string\",\n      \"description\": \"The postal code of the primary address.\"\n    },\n\
  \    \"address1_country\": {\n      \"type\": \"string\",\n      \"description\": \"The country of the primary address.\"\n    },\n    \"birthdate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date of birth of the contact.\"\n    },\n    \"statecode\": {\n      \"type\": \"integer\",\n      \"description\": \"The state of the contact (0 = Active, 1 = Inactive).\"\n    },\n    \"statuscode\": {\n      \"type\": \"integer\",\n      \"description\": \"The status reason code.\"\n    },\n    \"createdon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the contact was created.\",\n      \"readOnly\": true\n    },\n    \"modifiedon\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the contact was last modified.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"lastname\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dynamics/refs/heads/main/json-schema/contact.json
tags:
- CRM
- ERP
- Microsoft Dynamics
title: Contact
---
