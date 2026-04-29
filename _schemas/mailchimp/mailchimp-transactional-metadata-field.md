---
description: A custom metadata field definition.
layout: schema
name: MetadataField
properties_list:
- description: The unique name of the metadata field.
  name: name
  type: string
- description: The current state of the field.
  name: state
  type: string
- description: The Mustache template for displaying the field in the UI.
  name: view_template
  type: string
provider_name: Mailchimp
provider_slug: mailchimp
schema_file: json-schema/mailchimp-transactional-metadata-field-schema.json
slug: mailchimp-transactional-metadata-field
source_filename: mailchimp-transactional-metadata-field-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetadataField\",\n  \"type\": \"object\",\n  \"description\": \"A custom metadata field definition.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the metadata field.\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"The current state of the field.\"\n    },\n    \"view_template\": {\n      \"type\": \"string\",\n      \"description\": \"The Mustache template for displaying the field in the UI.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mailchimp/refs/heads/main/json-schema/mailchimp-transactional-metadata-field-schema.json
tags:
- Campaigns
- Email Marketing
- Marketing Automation
- Newsletters
- Transactional Email
title: MetadataField
---
