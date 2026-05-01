---
description: Schema for a reCAPTCHA Enterprise assessment request and response, used to evaluate risk scores for user interactions.
layout: schema
name: reCAPTCHA Enterprise Assessment
properties_list:
- description: The resource name of the assessment (output only)
  name: name
  type: string
- description: ''
  name: event
  type: object
- description: ''
  name: riskAnalysis
  type: object
- description: ''
  name: tokenProperties
  type: object
provider_name: Google reCAPTCHA
provider_slug: google-recaptcha
schema_file: json-schema/google-recaptcha-assessment-schema.json
slug: google-recaptcha-assessment
source_filename: google-recaptcha-assessment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/recaptcha-enterprise/assessment.json\",\n  \"title\": \"reCAPTCHA Enterprise Assessment\",\n  \"description\": \"Schema for a reCAPTCHA Enterprise assessment request and response, used to evaluate risk scores for user interactions.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The resource name of the assessment (output only)\",\n      \"readOnly\": true\n    },\n    \"event\": {\n      \"$ref\": \"#/$defs/Event\"\n    },\n    \"riskAnalysis\": {\n      \"$ref\": \"#/$defs/RiskAnalysis\"\n    },\n    \"tokenProperties\": {\n      \"$ref\": \"#/$defs/TokenProperties\"\n    }\n  },\n  \"$defs\": {\n    \"Event\": {\n      \"type\": \"object\",\n      \"description\": \"The event being assessed\",\n      \"required\": [\"token\", \"siteKey\"],\n      \"properties\": {\n        \"token\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The reCAPTCHA token provided by the client-side integration\"\n        },\n        \"siteKey\": {\n          \"type\": \"string\",\n          \"description\": \"The site key that was used to invoke reCAPTCHA\"\n        },\n        \"userAgent\": {\n          \"type\": \"string\",\n          \"description\": \"The user agent from the request\"\n        },\n        \"userIpAddress\": {\n          \"type\": \"string\",\n          \"description\": \"The IP address of the user\"\n        },\n        \"expectedAction\": {\n          \"type\": \"string\",\n          \"description\": \"The expected action for this interaction\"\n        }\n      }\n    },\n    \"RiskAnalysis\": {\n      \"type\": \"object\",\n      \"description\": \"Risk analysis result for the assessment\",\n      \"properties\": {\n        \"score\": {\n          \"type\": \"number\",\n          \"description\": \"Legitimacy score from 0.0 (likely bot) to 1.0 (likely\
  \ human)\",\n          \"minimum\": 0.0,\n          \"maximum\": 1.0\n        },\n        \"reasons\": {\n          \"type\": \"array\",\n          \"description\": \"Reasons contributing to the risk analysis\",\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"AUTOMATION\",\n              \"UNEXPECTED_ENVIRONMENT\",\n              \"TOO_MUCH_TRAFFIC\",\n              \"UNEXPECTED_USAGE_PATTERNS\",\n              \"LOW_CONFIDENCE_SCORE\"\n            ]\n          }\n        }\n      }\n    },\n    \"TokenProperties\": {\n      \"type\": \"object\",\n      \"description\": \"Properties of the submitted reCAPTCHA token\",\n      \"properties\": {\n        \"valid\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the token is valid\"\n        },\n        \"hostname\": {\n          \"type\": \"string\",\n          \"description\": \"The hostname of the page where the token was generated\"\n        },\n        \"\
  action\": {\n          \"type\": \"string\",\n          \"description\": \"The action name provided when the token was generated\"\n        },\n        \"createTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the token was generated\"\n        },\n        \"invalidReason\": {\n          \"type\": \"string\",\n          \"description\": \"Reason the token is invalid, if applicable\",\n          \"enum\": [\"EXPIRED\", \"DUPE\", \"MISSING\", \"BROWSER_ERROR\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-recaptcha/refs/heads/main/json-schema/google-recaptcha-assessment-schema.json
tags:
- Abuse Prevention
- Bot Detection
- CAPTCHA
- Fraud Prevention
- Google Cloud
- Security
title: reCAPTCHA Enterprise Assessment
---
