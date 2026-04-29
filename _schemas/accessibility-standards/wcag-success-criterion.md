---
description: A WCAG success criterion defining a testable requirement for accessible web content.
layout: schema
name: WcagSuccessCriterion
properties_list:
- description: The WCAG success criterion identifier, e.g. 1.1.1
  name: id
  type: string
- description: Short name of the success criterion
  name: title
  type: string
- description: Conformance level of the success criterion
  name: level
  type: string
- description: The POUR principle the criterion belongs to
  name: principle
  type: string
- description: The guideline number the criterion belongs to
  name: guideline
  type: string
- description: Full text of the success criterion requirement
  name: description
  type: string
- description: URL to the official WCAG success criterion documentation
  name: url
  type: string
- description: WCAG version that introduced this criterion
  name: version
  type: string
- description: URL to the understanding document for this criterion
  name: understanding
  type: string
- description: List of technique identifiers applicable to this criterion
  name: techniques
  type: array
provider_name: Accessibility Standards
provider_slug: accessibility-standards
schema_file: json-schema/wcag-success-criterion-schema.json
slug: wcag-success-criterion
source_filename: wcag-success-criterion-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accessibility-standards/refs/heads/main/json-schema/wcag-success-criterion-schema.json\",\n  \"title\": \"WcagSuccessCriterion\",\n  \"description\": \"A WCAG success criterion defining a testable requirement for accessible web content.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The WCAG success criterion identifier, e.g. 1.1.1\",\n      \"example\": \"1.1.1\",\n      \"pattern\": \"^[0-9]+\\\\.[0-9]+\\\\.[0-9]+$\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Short name of the success criterion\",\n      \"example\": \"Non-text Content\"\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"description\": \"Conformance level of the success criterion\",\n      \"enum\": [\"A\", \"AA\", \"AAA\"],\n      \"example\": \"A\"\n   \
  \ },\n    \"principle\": {\n      \"type\": \"string\",\n      \"description\": \"The POUR principle the criterion belongs to\",\n      \"enum\": [\"Perceivable\", \"Operable\", \"Understandable\", \"Robust\"],\n      \"example\": \"Perceivable\"\n    },\n    \"guideline\": {\n      \"type\": \"string\",\n      \"description\": \"The guideline number the criterion belongs to\",\n      \"example\": \"1.1\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Full text of the success criterion requirement\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the official WCAG success criterion documentation\",\n      \"example\": \"https://www.w3.org/TR/WCAG22/#non-text-content\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"WCAG version that introduced this criterion\",\n      \"example\": \"2.0\"\n    },\n    \"understanding\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"uri\",\n      \"description\": \"URL to the understanding document for this criterion\"\n    },\n    \"techniques\": {\n      \"type\": \"array\",\n      \"description\": \"List of technique identifiers applicable to this criterion\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"G94\", \"H37\", \"C9\"]\n    }\n  },\n  \"required\": [\"id\", \"title\", \"level\", \"principle\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accessibility-standards/refs/heads/main/json-schema/wcag-success-criterion-schema.json
tags:
- Accessibility
- Compliance
- UX
- Web Standards
- WCAG
- ARIA
- Section 508
- Disability
title: WcagSuccessCriterion
---
