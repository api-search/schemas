---
description: A Person in Salesloft represents a contact or prospect being engaged through the sales process.
layout: schema
name: Salesloft Person
properties_list:
- description: Unique identifier for the person
  name: id
  type: integer
- description: First name of the person
  name: first_name
  type: string
- description: Last name of the person
  name: last_name
  type: string
- description: Primary email address
  name: email_address
  type: string
- description: Secondary email address
  name: secondary_email_address
  type: string
- description: Personal email address
  name: personal_email_address
  type: string
- description: Primary phone number
  name: phone
  type: string
- description: Phone extension
  name: phone_extension
  type: string
- description: Mobile phone number
  name: mobile_phone
  type: string
- description: Home phone number
  name: home_phone
  type: string
- description: LinkedIn profile URL
  name: linkedin_url
  type: string
- description: Job title of the person
  name: title
  type: string
- description: City
  name: city
  type: string
- description: State or province
  name: state
  type: string
- description: Country
  name: country
  type: string
- description: Work city
  name: work_city
  type: string
- description: Work state
  name: work_state
  type: string
- description: Work country
  name: work_country
  type: string
- description: Company name associated with this person
  name: person_company_name
  type: string
- description: Company website for this person
  name: person_company_website
  type: string
- description: Company industry for this person
  name: person_company_industry
  type: string
- description: Seniority level of the person's role
  name: job_seniority
  type: string
- description: Whether this person is flagged as do not contact
  name: do_not_contact
  type: boolean
- description: Whether this person is an EU resident (GDPR)
  name: eu_resident
  type: boolean
- description: Locale (e.g. en_US)
  name: locale
  type: string
- description: Personal website URL
  name: personal_website
  type: string
- description: Twitter handle
  name: twitter_handle
  type: string
- description: Array of tags
  name: tags
  type: array
- description: Contact restriction types (e.g. call, email)
  name: contact_restrictions
  type: array
- description: Custom field key-value pairs
  name: custom_fields
  type: object
- description: ID of the associated Account
  name: account_id
  type: integer
- description: ID of the user who owns this person
  name: owner_id
  type: integer
- description: ID of the import this person came from
  name: import_id
  type: integer
- description: ID of the person's current stage
  name: person_stage_id
  type: integer
- description: External CRM identifier
  name: crm_id
  type: string
- description: Type of external CRM
  name: crm_id_type
  type: string
- description: Timestamp when the person was created
  name: created_at
  type: string
- description: Timestamp when the person was last updated
  name: updated_at
  type: string
provider_name: Salesloft
provider_slug: salesloft
schema_file: json-schema/salesloft-person-schema.json
slug: salesloft-person
source_filename: salesloft-person-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/salesloft/json-schema/salesloft-person-schema.json\",\n  \"title\": \"Salesloft Person\",\n  \"description\": \"A Person in Salesloft represents a contact or prospect being engaged through the sales process.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique identifier for the person\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name of the person\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the person\"\n    },\n    \"email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Primary email address\"\n    },\n    \"secondary_email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Secondary email\
  \ address\"\n    },\n    \"personal_email_address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Personal email address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Primary phone number\"\n    },\n    \"phone_extension\": {\n      \"type\": \"string\",\n      \"description\": \"Phone extension\"\n    },\n    \"mobile_phone\": {\n      \"type\": \"string\",\n      \"description\": \"Mobile phone number\"\n    },\n    \"home_phone\": {\n      \"type\": \"string\",\n      \"description\": \"Home phone number\"\n    },\n    \"linkedin_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"LinkedIn profile URL\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title of the person\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"description\": \"City\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"State or province\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"Country\"\n    },\n    \"work_city\": {\n      \"type\": \"string\",\n      \"description\": \"Work city\"\n    },\n    \"work_state\": {\n      \"type\": \"string\",\n      \"description\": \"Work state\"\n    },\n    \"work_country\": {\n      \"type\": \"string\",\n      \"description\": \"Work country\"\n    },\n    \"person_company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name associated with this person\"\n    },\n    \"person_company_website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Company website for this person\"\n    },\n    \"person_company_industry\": {\n      \"type\": \"string\",\n      \"description\": \"Company industry for this person\"\n    },\n    \"job_seniority\": {\n      \"type\": \"string\",\n      \"description\": \"Seniority level of the person's role\",\n      \"enum\": [\"individual_contributor\"\
  , \"manager\", \"director\", \"vp\", \"c_suite\", \"owner\", \"unknown\"]\n    },\n    \"do_not_contact\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this person is flagged as do not contact\"\n    },\n    \"eu_resident\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this person is an EU resident (GDPR)\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"Locale (e.g. en_US)\"\n    },\n    \"personal_website\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Personal website URL\"\n    },\n    \"twitter_handle\": {\n      \"type\": \"string\",\n      \"description\": \"Twitter handle\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Array of tags\"\n    },\n    \"contact_restrictions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\"\
  : \"Contact restriction types (e.g. call, email)\"\n    },\n    \"custom_fields\": {\n      \"type\": \"object\",\n      \"description\": \"Custom field key-value pairs\",\n      \"additionalProperties\": true\n    },\n    \"account_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the associated Account\"\n    },\n    \"owner_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the user who owns this person\"\n    },\n    \"import_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the import this person came from\"\n    },\n    \"person_stage_id\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of the person's current stage\"\n    },\n    \"crm_id\": {\n      \"type\": \"string\",\n      \"description\": \"External CRM identifier\"\n    },\n    \"crm_id_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of external CRM\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Timestamp when the person was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the person was last updated\"\n    }\n  },\n  \"required\": [\"id\", \"email_address\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesloft/refs/heads/main/json-schema/salesloft-person-schema.json
tags:
- Sales
- CRM
- Revenue
- Automation
- AI
title: Salesloft Person
---
