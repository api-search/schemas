---
description: A WAI-ARIA role definition that provides semantic meaning to HTML elements for assistive technologies.
layout: schema
name: AriaRole
properties_list:
- description: The ARIA role name
  name: name
  type: string
- description: The role category in the ARIA taxonomy
  name: category
  type: string
- description: Description of the role and its semantic meaning
  name: description
  type: string
- description: Parent roles in the ARIA role hierarchy
  name: superclassRole
  type: array
- description: ARIA states required for this role
  name: requiredStates
  type: array
- description: ARIA properties supported by this role
  name: supportedProperties
  type: array
- description: HTML elements that natively carry this role
  name: implicitAriaSemantics
  type: string
- description: URL to the WAI-ARIA spec definition
  name: specUrl
  type: string
provider_name: Accessibility Standards
provider_slug: accessibility-standards
schema_file: json-schema/aria-role-schema.json
slug: aria-role
source_filename: aria-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accessibility-standards/refs/heads/main/json-schema/aria-role-schema.json\",\n  \"title\": \"AriaRole\",\n  \"description\": \"A WAI-ARIA role definition that provides semantic meaning to HTML elements for assistive technologies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The ARIA role name\",\n      \"example\": \"button\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The role category in the ARIA taxonomy\",\n      \"enum\": [\"Abstract\", \"Widget\", \"Document Structure\", \"Landmark\", \"Live Region\", \"Window\"],\n      \"example\": \"Widget\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the role and its semantic meaning\"\n    },\n    \"superclassRole\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"Parent roles in the ARIA role hierarchy\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"command\", \"input\"]\n    },\n    \"requiredStates\": {\n      \"type\": \"array\",\n      \"description\": \"ARIA states required for this role\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"aria-pressed\"]\n    },\n    \"supportedProperties\": {\n      \"type\": \"array\",\n      \"description\": \"ARIA properties supported by this role\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"aria-expanded\", \"aria-haspopup\", \"aria-label\"]\n    },\n    \"implicitAriaSemantics\": {\n      \"type\": \"string\",\n      \"description\": \"HTML elements that natively carry this role\",\n      \"example\": \"button, input[type=button]\"\n    },\n    \"specUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the\
  \ WAI-ARIA spec definition\",\n      \"example\": \"https://www.w3.org/TR/wai-aria-1.2/#button\"\n    }\n  },\n  \"required\": [\"name\", \"category\", \"description\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accessibility-standards/refs/heads/main/json-schema/aria-role-schema.json
tags:
- Accessibility
- Compliance
- UX
- Web Standards
- WCAG
- ARIA
- Section 508
- Disability
title: AriaRole
---
