---
description: Configuration for onsite application collection
layout: schema
name: OnsiteApplyConfiguration
properties_list:
- description: Webhook URL for receiving job applications
  name: jobApplicationWebhookUrl
  type: string
- description: ''
  name: questions
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-onsite-apply-configuration-schema.json
slug: linkedin-talent-job-posting-onsite-apply-configuration
source_filename: linkedin-talent-job-posting-onsite-apply-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-onsite-apply-configuration-schema.json\",\n  \"title\": \"OnsiteApplyConfiguration\",\n  \"description\": \"Configuration for onsite application collection\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobApplicationWebhookUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Webhook URL for receiving job applications\",\n      \"example\": \"https://ats.company.com/webhooks/linkedin-applications\"\n    },\n    \"questions\": {\n      \"$ref\": \"#/components/schemas/ApplicationQuestions\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-onsite-apply-configuration-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: OnsiteApplyConfiguration
---
