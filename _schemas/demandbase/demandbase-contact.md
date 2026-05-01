---
description: Represents a business contact in Demandbase with professional details, company association, and contact information for B2B engagement.
layout: schema
name: Demandbase Contact
properties_list:
- description: Unique Demandbase contact identifier
  name: contact_id
  type: string
- description: First name
  name: first_name
  type: string
- description: Last name
  name: last_name
  type: string
- description: Business email address
  name: email
  type: string
- description: Job title
  name: title
  type: string
- description: Department or functional area
  name: department
  type: string
- description: Seniority level (e.g., C-Level, VP, Director, Manager)
  name: seniority
  type: string
- description: Direct phone number
  name: phone
  type: string
- description: LinkedIn profile URL
  name: linkedin_url
  type: string
- description: Associated Demandbase company ID
  name: company_id
  type: string
- description: Company name
  name: company_name
  type: string
- description: Company web domain
  name: company_domain
  type: string
provider_name: Demandbase
provider_slug: demandbase
schema_file: json-schema/demandbase-contact-schema.json
slug: demandbase-contact
source_filename: demandbase-contact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.demandbase.com/schemas/demandbase/contact.json\",\n  \"title\": \"Demandbase Contact\",\n  \"description\": \"Represents a business contact in Demandbase with professional details, company association, and contact information for B2B engagement.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"contact_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Demandbase contact identifier\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"First name\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Business email address\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Job title\"\n    },\n    \"department\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Department or functional area\"\n    },\n    \"seniority\": {\n      \"type\": \"string\",\n      \"description\": \"Seniority level (e.g., C-Level, VP, Director, Manager)\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"description\": \"Direct phone number\"\n    },\n    \"linkedin_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"LinkedIn profile URL\"\n    },\n    \"company_id\": {\n      \"type\": \"string\",\n      \"description\": \"Associated Demandbase company ID\"\n    },\n    \"company_name\": {\n      \"type\": \"string\",\n      \"description\": \"Company name\"\n    },\n    \"company_domain\": {\n      \"type\": \"string\",\n      \"description\": \"Company web domain\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/demandbase/refs/heads/main/json-schema/demandbase-contact-schema.json
tags:
- Account-Based Marketing
- Advertising
- AI Agents
- B2B Marketing
- Data Enrichment
- Intent Data
- Personalization
- Sales Intelligence
title: Demandbase Contact
---
