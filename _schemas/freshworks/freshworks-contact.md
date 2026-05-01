---
description: A contact record representing a customer, requester, or lead across Freshworks products including Freshdesk, Freshsales, and Freshchat. Contacts are the primary person entities in the Freshworks ecosystem.
layout: schema
name: Freshworks Contact
properties_list:
- description: Unique identifier of the contact.
  name: id
  type: integer
- description: First name of the contact.
  name: first_name
  type: string
- description: Last name of the contact.
  name: last_name
  type: string
- description: Full display name of the contact.
  name: name
  type: string
- description: Primary email address of the contact.
  name: email
  type: string
- description: Primary phone number.
  name: phone
  type: string
- description: Mobile phone number.
  name: mobile
  type: string
- description: Mailing or street address.
  name: address
  type: string
- description: City of residence.
  name: city
  type: string
- description: State or province.
  name: state
  type: string
- description: Country of residence.
  name: country
  type: string
- description: ZIP or postal code.
  name: zipcode
  type: string
- description: Job title or position.
  name: job_title
  type: string
- description: Department within the company.
  name: department
  type: string
- description: ID of the associated company or account.
  name: company_id
  type: integer
- description: Name of the associated company.
  name: company_name
  type: string
- description: Preferred language (ISO 639-1 code).
  name: language
  type: string
- description: Time zone identifier (IANA format).
  name: time_zone
  type: string
- description: Tags applied to the contact for segmentation.
  name: tags
  type: array
- description: Whether the contact is active in the system.
  name: active
  type: boolean
- description: Lead score assigned to the contact (Freshsales).
  name: lead_score
  type: integer
- description: ID of the sales agent who owns this contact (Freshsales).
  name: owner_id
  type: integer
- description: Custom field key-value pairs specific to the account configuration.
  name: custom_fields
  type: object
- description: Timestamp when the contact was created.
  name: created_at
  type: string
- description: Timestamp when the contact was last updated.
  name: updated_at
  type: string
provider_name: freshworks
provider_slug: freshworks
schema_file: json-schema/freshworks-contact-schema.json
slug: freshworks-contact
source_filename: freshworks-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://freshworks.com/schemas/freshworks/contact.json\",\n  \"title\": \"Freshworks Contact\",\n  \"description\": \"A contact record representing a customer, requester, or lead across Freshworks products including Freshdesk, Freshsales, and Freshchat. Contacts are the primary person entities in the Freshworks ecosystem.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier of the contact.\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the contact.\",\n      \"maxLength\": 255\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the contact.\",\n      \"maxLength\": 255\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the contact.\",\n\
  \      \"maxLength\": 255\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address of the contact.\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number.\",\n      \"pattern\": \"^[+]?[0-9\\\\s\\\\-().]+$\"\n    },\n    \"mobile\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number.\",\n      \"pattern\": \"^[+]?[0-9\\\\s\\\\-().]+$\"\n    },\n    \"address\": {\n      \"type\": \"string\",\n      \"description\": \"Mailing or street address.\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City of residence.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"State or province.\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country of residence.\"\n    },\n    \"zipcode\": {\n      \"type\": \"string\",\n      \"description\": \"ZIP or\
  \ postal code.\"\n    },\n    \"job_title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title or position.\"\n    },\n    \"department\": {\n      \"type\": \"string\",\n      \"description\": \"Department within the company.\"\n    },\n    \"company_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the associated company or account.\"\n    },\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the associated company.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Preferred language (ISO 639-1 code).\",\n      \"pattern\": \"^[a-z]{2}(-[A-Z]{2})?$\"\n    },\n    \"time_zone\": {\n      \"type\": \"string\",\n      \"description\": \"Time zone identifier (IANA format).\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags applied to the contact for segmentation.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"active\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the contact is active in the system.\"\n    },\n    \"lead_score\": {\n      \"type\": \"integer\",\n      \"description\": \"Lead score assigned to the contact (Freshsales).\",\n      \"minimum\": 0\n    },\n    \"owner_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the sales agent who owns this contact (Freshsales).\"\n    },\n    \"custom_fields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom field key-value pairs specific to the account configuration.\",\n      \"additionalProperties\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the contact was created.\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the contact was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/freshworks/refs/heads/main/json-schema/freshworks-contact-schema.json
tags: []
title: Freshworks Contact
---
