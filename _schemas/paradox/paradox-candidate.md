---
description: JSON Schema for a candidate resource in the Paradox conversational AI recruiting platform. Candidates represent individuals progressing through automated screening, interview scheduling, and hiring workflows powered by the Olivia AI assistant.
layout: schema
name: Paradox Candidate
properties_list:
- description: Unique internal candidate identifier assigned by Paradox
  name: OID
  type: integer
- description: Encrypted external candidate identifier
  name: external_oid
  type: string
- description: Full name of the candidate (required if first_name/last_name not provided)
  name: name
  type: string
- description: First name of the candidate (use with last_name instead of name)
  name: first_name
  type: string
- description: Last name of the candidate (use with first_name instead of name)
  name: last_name
  type: string
- description: Candidate email address
  name: email
  type: string
- description: Candidate phone number with country code
  name: phone
  type: string
- description: External candidate identifier from an integrated system
  name: ex_id
  type: string
- description: External status designation from an integrated system
  name: ex_status
  type: string
- description: External step designation from an integrated system
  name: ex_step
  type: string
- description: External reason designation from an integrated system
  name: ex_reason
  type: string
- description: Job requisition identifier the candidate is associated with
  name: job_req_id
  type: string
- description: Job position title the candidate is applying for
  name: job_title
  type: string
- description: Job location code identifying the candidate work site
  name: job_loc_code
  type: string
- description: 'Preferred contact method: 1=Email, 2=SMS, 3=Email & SMS, 4=WhatsApp & Email, 5=WhatsApp'
  name: primary_contact_method
  type: integer
- description: Employment start date (ISO 8601 format)
  name: hired_date
  type:
  - string
  - 'null'
- description: HireVue virtual interview link
  name: hirevue_link
  type: string
- description: Pymetrics assessment platform link
  name: pymetrics_link
  type: string
- description: ADP workforce management system link
  name: adp_link
  type: string
- description: Interview guidance text provided to the candidate
  name: hirevue_instructions
  type: string
- description: Candidate tier classification for segmentation
  name: audience_type
  type: string
- description: Hirescore candidate identifier
  name: hm_cid
  type: string
- description: Group classification identifier for organizing candidates
  name: external_group_id
  type: string
- description: Email address of the person who referred the candidate
  name: referrer_email
  type: string
- description: Name of the person who referred the candidate
  name: referrer_name
  type: string
- description: Email of the assigned recruiter
  name: recruiter_email
  type: string
- description: Contact information for the assigned hiring manager
  name: hiring_manager
  type: string
- description: External referral source information
  name: external_referrer
  type: string
- description: Candidate language preference code (e.g. en, es, fr)
  name: language_preference
  type: string
- description: Name of the journey workflow the candidate is enrolled in
  name: candidate_journey
  type: string
- description: Current stage designation within the candidate journey
  name: candidate_journey_status
  type: string
- description: Custom candidate attributes as key-value pairs (values limited to 255 characters each)
  name: candidate_attribute_data
  type: object
- description: Application identifier for the candidate
  name: job_application_id
  type: string
- description: Whether to use the application ID to identify returning candidates
  name: use_application_id_for_identity
  type: boolean
- description: Geographic location information for the candidate
  name: candidate_location_info
  type: string
- description: Source system identifier indicating where the candidate originated
  name: external_source_id
  type: string
- description: Filename of the attached offer letter document
  name: offer_file_name
  type: string
- description: Whether to enable Paradox status mapping
  name: use_paradox_status_map
  type: boolean
- description: Paradox journey status name for status mapping
  name: status_map_name
  type: string
- description: External system status identifier for status mapping
  name: status_map_ex_id
  type: string
- description: Whether the candidate is added to the talent pool
  name: talent_community
  type: boolean
- description: Community identifier when talent_community is true
  name: community_of_interest
  type: integer
- description: Whether to bypass opt-in messaging
  name: skip_send_opt_in
  type: boolean
- description: Marketing consent status for the candidate
  name: consent_to_marketing
  type: string
- description: Internal notes about the candidate
  name: note
  type: string
provider_name: Paradox
provider_slug: paradox
schema_file: json-schema/paradox-candidate-schema.json
slug: paradox-candidate
source_filename: paradox-candidate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"paradox-candidate-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Paradox Candidate\",\n  \"description\": \"JSON Schema for a candidate resource in the Paradox conversational AI recruiting platform. Candidates represent individuals progressing through automated screening, interview scheduling, and hiring workflows powered by the Olivia AI assistant.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"phone\",\n    \"email\"\n  ],\n  \"properties\": {\n    \"OID\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique internal candidate identifier assigned by Paradox\"\n    },\n    \"external_oid\": {\n      \"type\": \"string\",\n      \"description\": \"Encrypted external candidate identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"Full name of the candidate (required if first_name/last_name not provided)\"\n    },\n    \"first_name\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"First name of the candidate (use with last_name instead of name)\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Last name of the candidate (use with first_name instead of name)\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"maxLength\": 50,\n      \"description\": \"Candidate email address\"\n    },\n    \"phone\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"Candidate phone number with country code\"\n    },\n    \"ex_id\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"External candidate identifier from an integrated system\"\n    },\n    \"ex_status\": {\n      \"type\": \"string\",\n      \"description\": \"External status designation from an integrated system\"\n    },\n    \"ex_step\": {\n      \"type\": \"string\",\n      \"description\": \"External step designation\
  \ from an integrated system\"\n    },\n    \"ex_reason\": {\n      \"type\": \"string\",\n      \"description\": \"External reason designation from an integrated system\"\n    },\n    \"job_req_id\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Job requisition identifier the candidate is associated with\"\n    },\n    \"job_title\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Job position title the candidate is applying for\"\n    },\n    \"job_loc_code\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"Job location code identifying the candidate work site\"\n    },\n    \"primary_contact_method\": {\n      \"type\": \"integer\",\n      \"enum\": [1, 2, 3, 4, 5],\n      \"description\": \"Preferred contact method: 1=Email, 2=SMS, 3=Email & SMS, 4=WhatsApp & Email, 5=WhatsApp\"\n    },\n    \"hired_date\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"Employment start date (ISO 8601 format)\"\n    },\n    \"hirevue_link\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"format\": \"uri\",\n      \"description\": \"HireVue virtual interview link\"\n    },\n    \"pymetrics_link\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"format\": \"uri\",\n      \"description\": \"Pymetrics assessment platform link\"\n    },\n    \"adp_link\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"format\": \"uri\",\n      \"description\": \"ADP workforce management system link\"\n    },\n    \"hirevue_instructions\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Interview guidance text provided to the candidate\"\n    },\n    \"audience_type\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Candidate tier classification for segmentation\"\n    },\n    \"hm_cid\": {\n      \"type\": \"string\"\
  ,\n      \"maxLength\": 255,\n      \"description\": \"Hirescore candidate identifier\"\n    },\n    \"external_group_id\": {\n      \"type\": \"string\",\n      \"description\": \"Group classification identifier for organizing candidates\"\n    },\n    \"referrer_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"maxLength\": 50,\n      \"description\": \"Email address of the person who referred the candidate\"\n    },\n    \"referrer_name\": {\n      \"type\": \"string\",\n      \"maxLength\": 50,\n      \"description\": \"Name of the person who referred the candidate\"\n    },\n    \"recruiter_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email of the assigned recruiter\"\n    },\n    \"hiring_manager\": {\n      \"type\": \"string\",\n      \"description\": \"Contact information for the assigned hiring manager\"\n    },\n    \"external_referrer\": {\n      \"type\": \"string\",\n      \"maxLength\": 1000,\n\
  \      \"description\": \"External referral source information\"\n    },\n    \"language_preference\": {\n      \"type\": \"string\",\n      \"default\": \"en\",\n      \"description\": \"Candidate language preference code (e.g. en, es, fr)\"\n    },\n    \"candidate_journey\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the journey workflow the candidate is enrolled in\"\n    },\n    \"candidate_journey_status\": {\n      \"type\": \"string\",\n      \"description\": \"Current stage designation within the candidate journey\"\n    },\n    \"candidate_attribute_data\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"maxLength\": 255\n      },\n      \"description\": \"Custom candidate attributes as key-value pairs (values limited to 255 characters each)\"\n    },\n    \"job_application_id\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Application identifier for the candidate\"\
  \n    },\n    \"use_application_id_for_identity\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to use the application ID to identify returning candidates\"\n    },\n    \"candidate_location_info\": {\n      \"type\": \"string\",\n      \"maxLength\": 100,\n      \"description\": \"Geographic location information for the candidate\"\n    },\n    \"external_source_id\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"description\": \"Source system identifier indicating where the candidate originated\"\n    },\n    \"offer_file_name\": {\n      \"type\": \"string\",\n      \"maxLength\": 150,\n      \"description\": \"Filename of the attached offer letter document\"\n    },\n    \"use_paradox_status_map\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether to enable Paradox status mapping\"\n    },\n    \"status_map_name\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Paradox journey status name for status mapping\"\n    },\n    \"status_map_ex_id\": {\n      \"type\": \"string\",\n      \"description\": \"External system status identifier for status mapping\"\n    },\n    \"talent_community\": {\n      \"type\": \"boolean\",\n      \"default\": false,\n      \"description\": \"Whether the candidate is added to the talent pool\"\n    },\n    \"community_of_interest\": {\n      \"type\": \"integer\",\n      \"description\": \"Community identifier when talent_community is true\"\n    },\n    \"skip_send_opt_in\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to bypass opt-in messaging\"\n    },\n    \"consent_to_marketing\": {\n      \"type\": \"string\",\n      \"description\": \"Marketing consent status for the candidate\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"description\": \"Internal notes about the candidate\"\n    }\n  },\n  \"oneOf\": [\n    {\n      \"required\": [\"name\"]\n    },\n    {\n      \"\
  required\": [\"first_name\", \"last_name\"]\n    }\n  ],\n  \"examples\": [\n    {\n      \"name\": \"Jane Smith\",\n      \"email\": \"jane.smith@example.com\",\n      \"phone\": \"+15551234567\",\n      \"job_req_id\": \"REQ-2026-001\",\n      \"job_title\": \"Software Engineer\",\n      \"job_loc_code\": \"US-NY-100\",\n      \"primary_contact_method\": 3,\n      \"language_preference\": \"en\",\n      \"candidate_journey\": \"Standard Hiring\",\n      \"candidate_attribute_data\": {\n        \"years_experience\": \"5\",\n        \"degree\": \"BS Computer Science\"\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/paradox/refs/heads/main/json-schema/paradox-candidate-schema.json
tags:
- Artificial Intelligence
- Candidate Screening
- Chatbot
- Conversational AI
- Hiring Automation
- HR Technology
- Interview Scheduling
- Recruiting
- SMS
- Talent Acquisition
title: Paradox Candidate
---
