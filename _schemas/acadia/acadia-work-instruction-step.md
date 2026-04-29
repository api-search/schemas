---
description: A single step within a work instruction
layout: schema
name: WorkInstructionStep
properties_list:
- description: Step sequence number
  name: order
  type: integer
- description: Step title
  name: title
  type: string
- description: Detailed description of the step
  name: description
  type: string
provider_name: Acadia
provider_slug: acadia
schema_file: json-schema/acadia-work-instruction-step-schema.json
slug: acadia-work-instruction-step
source_filename: acadia-work-instruction-step-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-work-instruction-step-schema.json\",\n  \"title\": \"WorkInstructionStep\",\n  \"description\": \"A single step within a work instruction\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"Step sequence number\",\n      \"example\": 1\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Step title\",\n      \"example\": \"Inspect Machine\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the step\",\n      \"example\": \"Visually inspect the machine for defects or hazards\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acadia/refs/heads/main/json-schema/acadia-work-instruction-step-schema.json
tags:
- Connected Worker
- Knowledge Management
- Manufacturing
- Skills Management
- Training
- Workforce Development
title: WorkInstructionStep
---
