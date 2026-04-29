---
description: Input for creating or updating an employer on Indeed.
layout: schema
name: PatchEmployerInput
properties_list:
- description: A globally unique employer identifier composed of the ATS identifier and the employer's ID within that system.
  name: id
  type: string
- description: The employer's display name. Required when creating a new employer, optional when updating an existing one.
  name: employerName
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-patch-employer-input-schema.json
slug: indeed-employer-patch-employer-input
source_filename: indeed-employer-patch-employer-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PatchEmployerInput\",\n  \"type\": \"object\",\n  \"description\": \"Input for creating or updating an employer on Indeed.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A globally unique employer identifier composed of the ATS identifier and the employer's ID within that system.\"\n    },\n    \"employerName\": {\n      \"type\": \"string\",\n      \"description\": \"The employer's display name. Required when creating a new employer, optional when updating an existing one.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-patch-employer-input-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: PatchEmployerInput
---
