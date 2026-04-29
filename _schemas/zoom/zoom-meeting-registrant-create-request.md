---
description: ''
layout: schema
name: RegistrantCreateRequest
properties_list:
- description: Registrant email address.
  name: email
  type: string
- description: Registrant first name.
  name: first_name
  type: string
- description: Registrant last name.
  name: last_name
  type: string
- description: Registrant address.
  name: address
  type: string
- description: Registrant city.
  name: city
  type: string
- description: Registrant state or province.
  name: state
  type: string
- description: Registrant zip or postal code.
  name: zip
  type: string
- description: Registrant two-letter country code.
  name: country
  type: string
- description: Registrant phone number.
  name: phone
  type: string
- description: Registrant questions and comments.
  name: comments
  type: string
- description: Registrant industry.
  name: industry
  type: string
- description: Registrant job title.
  name: job_title
  type: string
- description: Registrant organization.
  name: org
  type: string
- description: Number of employees.
  name: no_of_employees
  type: string
- description: Purchasing time frame.
  name: purchasing_time_frame
  type: string
- description: Role in purchase process.
  name: role_in_purchase_process
  type: string
- description: Registrant language preference.
  name: language
  type: string
- description: Custom question responses.
  name: custom_questions
  type: array
- description: Auto-approve this registrant.
  name: auto_approve
  type: boolean
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-registrant-create-request-schema.json
slug: zoom-meeting-registrant-create-request
source_filename: zoom-meeting-registrant-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RegistrantCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant email address.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant first name.\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant last name.\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant city.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant state or province.\"\n    },\n    \"zip\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant zip or postal code.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"Registrant two-letter country code.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant phone number.\"\n    },\n    \"comments\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant questions and comments.\"\n    },\n    \"industry\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant industry.\"\n    },\n    \"job_title\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant job title.\"\n    },\n    \"org\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant organization.\"\n    },\n    \"no_of_employees\": {\n      \"type\": \"string\",\n      \"description\": \"Number of employees.\"\n    },\n    \"purchasing_time_frame\": {\n      \"type\": \"string\",\n      \"description\": \"Purchasing time frame.\"\n    },\n    \"role_in_purchase_process\": {\n      \"type\": \"string\",\n      \"description\": \"Role in purchase process.\"\n    },\n    \"language\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Registrant language preference.\"\n    },\n    \"custom_questions\": {\n      \"type\": \"array\",\n      \"description\": \"Custom question responses.\"\n    },\n    \"auto_approve\": {\n      \"type\": \"boolean\",\n      \"description\": \"Auto-approve this registrant.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-registrant-create-request-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: RegistrantCreateRequest
---
