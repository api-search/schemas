---
description: Schema for a complaint record returned by the CCDB API.
layout: schema
name: CFPB Consumer Complaint
properties_list:
- description: ''
  name: complaint_id
  type: string
- description: ''
  name: date_received
  type: string
- description: ''
  name: date_sent_to_company
  type: string
- description: ''
  name: product
  type: string
- description: ''
  name: sub_product
  type: string
- description: ''
  name: issue
  type: string
- description: ''
  name: sub_issue
  type: string
- description: ''
  name: company
  type: string
- description: ''
  name: company_response
  type: string
- description: ''
  name: company_public_response
  type: string
- description: ''
  name: consumer_consent_provided
  type: string
- description: ''
  name: consumer_disputed
  type: string
- description: ''
  name: complaint_what_happened
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: zip_code
  type: string
- description: ''
  name: tags
  type: string
- description: ''
  name: timely
  type: string
- description: ''
  name: submitted_via
  type: string
provider_name: Consumer Financial Protection Bureau
provider_slug: consumer-financial-protection-bureau
schema_file: json-schema/cfpb-complaint-schema.json
slug: cfpb-complaint
source_filename: cfpb-complaint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/json-schema/cfpb-complaint-schema.json\",\n  \"title\": \"CFPB Consumer Complaint\",\n  \"description\": \"Schema for a complaint record returned by the CCDB API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"complaint_id\": { \"type\": \"string\" },\n    \"date_received\": { \"type\": \"string\", \"format\": \"date\" },\n    \"date_sent_to_company\": { \"type\": \"string\", \"format\": \"date\" },\n    \"product\": { \"type\": \"string\" },\n    \"sub_product\": { \"type\": \"string\" },\n    \"issue\": { \"type\": \"string\" },\n    \"sub_issue\": { \"type\": \"string\" },\n    \"company\": { \"type\": \"string\" },\n    \"company_response\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Closed\",\n        \"Closed with explanation\",\n        \"Closed with monetary relief\"\
  ,\n        \"Closed with non-monetary relief\",\n        \"Closed with relief\",\n        \"Closed without relief\",\n        \"In progress\",\n        \"Untimely response\"\n      ]\n    },\n    \"company_public_response\": { \"type\": \"string\" },\n    \"consumer_consent_provided\": { \"type\": \"string\" },\n    \"consumer_disputed\": { \"type\": \"string\" },\n    \"complaint_what_happened\": { \"type\": \"string\" },\n    \"state\": { \"type\": \"string\", \"minLength\": 2, \"maxLength\": 2 },\n    \"zip_code\": { \"type\": \"string\" },\n    \"tags\": { \"type\": \"string\" },\n    \"timely\": { \"type\": \"string\", \"enum\": [\"Yes\", \"No\"] },\n    \"submitted_via\": {\n      \"type\": \"string\",\n      \"enum\": [\"Web\", \"Phone\", \"Email\", \"Postal mail\", \"Fax\", \"Referral\"]\n    }\n  },\n  \"required\": [\"complaint_id\", \"date_received\", \"product\", \"company\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/consumer-financial-protection-bureau/refs/heads/main/json-schema/cfpb-complaint-schema.json
tags:
- Banking
- Complaints
- Consumer Protection
- Federal Government
- Financial Services
- HMDA
- Mortgages
- Open Data
title: CFPB Consumer Complaint
---
