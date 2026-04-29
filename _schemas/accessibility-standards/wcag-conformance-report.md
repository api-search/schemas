---
description: An accessibility conformance report documenting the evaluation of a website or application against WCAG criteria.
layout: schema
name: WcagConformanceReport
properties_list:
- description: Unique identifier for this conformance report
  name: id
  type: string
- description: The website or application being evaluated
  name: subject
  type: object
- description: The WCAG version evaluated against
  name: standard
  type: string
- description: The claimed conformance level
  name: conformanceLevel
  type: string
- description: Overall conformance status
  name: status
  type: string
- description: Date the evaluation was conducted
  name: evaluationDate
  type: string
- description: Name or organization that performed the evaluation
  name: evaluator
  type: string
- description: List of accessibility violations found
  name: violations
  type: array
provider_name: Accessibility Standards
provider_slug: accessibility-standards
schema_file: json-schema/wcag-conformance-report-schema.json
slug: wcag-conformance-report
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/accessibility-standards/refs/heads/main/json-schema/wcag-conformance-report-schema.json\",\n  \"title\": \"WcagConformanceReport\",\n  \"description\": \"An accessibility conformance report documenting the evaluation of a website or application against WCAG criteria.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for this conformance report\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"subject\": {\n      \"type\": \"object\",\n      \"description\": \"The website or application being evaluated\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the evaluated site or application\",\n          \"example\": \"Example Web Application\"\
  \n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the evaluated site\",\n          \"example\": \"https://www.example.com\"\n        }\n      },\n      \"required\": [\"name\", \"url\"]\n    },\n    \"standard\": {\n      \"type\": \"string\",\n      \"description\": \"The WCAG version evaluated against\",\n      \"enum\": [\"WCAG 2.0\", \"WCAG 2.1\", \"WCAG 2.2\", \"WCAG 3.0\"],\n      \"example\": \"WCAG 2.2\"\n    },\n    \"conformanceLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The claimed conformance level\",\n      \"enum\": [\"A\", \"AA\", \"AAA\"],\n      \"example\": \"AA\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall conformance status\",\n      \"enum\": [\"Passes\", \"Fails\", \"Partial\", \"Not Evaluated\"],\n      \"example\": \"Partial\"\n    },\n    \"evaluationDate\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date\",\n      \"description\": \"Date the evaluation was conducted\",\n      \"example\": \"2026-04-19\"\n    },\n    \"evaluator\": {\n      \"type\": \"string\",\n      \"description\": \"Name or organization that performed the evaluation\",\n      \"example\": \"Accessibility Consulting Group\"\n    },\n    \"violations\": {\n      \"type\": \"array\",\n      \"description\": \"List of accessibility violations found\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Violation\"\n      }\n    }\n  },\n  \"required\": [\"subject\", \"standard\", \"conformanceLevel\", \"evaluationDate\"],\n  \"$defs\": {\n    \"Violation\": {\n      \"type\": \"object\",\n      \"description\": \"A single accessibility violation found during evaluation\",\n      \"properties\": {\n        \"criterionId\": {\n          \"type\": \"string\",\n          \"description\": \"WCAG success criterion identifier\",\n          \"example\": \"1.4.3\"\n        },\n        \"severity\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"critical\", \"serious\", \"moderate\", \"minor\"],\n          \"example\": \"serious\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the violation\",\n          \"example\": \"Text contrast ratio of 2.5:1 does not meet minimum 4.5:1 requirement\"\n        },\n        \"element\": {\n          \"type\": \"string\",\n          \"description\": \"CSS selector or XPath of the offending element\",\n          \"example\": \".nav-link\"\n        },\n        \"remediation\": {\n          \"type\": \"string\",\n          \"description\": \"Recommended fix for the violation\"\n        }\n      },\n      \"required\": [\"criterionId\", \"severity\", \"description\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/accessibility-standards/refs/heads/main/json-schema/wcag-conformance-report-schema.json
tags:
- Accessibility
- Compliance
- UX
- Web Standards
- WCAG
- ARIA
- Section 508
- Disability
title: WcagConformanceReport
---
