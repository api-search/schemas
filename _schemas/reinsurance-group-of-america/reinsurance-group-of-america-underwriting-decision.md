---
description: Schema for an automated underwriting decision returned by RGA's AURA NEXT platform API.
layout: schema
name: AURA NEXT Underwriting Decision
properties_list:
- description: Unique identifier for the insurance application.
  name: applicationId
  type: string
- description: Unique identifier for this underwriting decision.
  name: decisionId
  type: string
- description: Timestamp when the underwriting decision was made.
  name: decisionDate
  type: string
- description: The underwriting decision outcome.
  name: decision
  type: string
- description: Assigned risk classification (e.g., 'Preferred Plus', 'Standard', 'Substandard').
  name: riskClass
  type: string
- description: Table rating if applicable (percentage above standard mortality, in multiples of 25).
  name: tableRating
  type: integer
- description: Flat extra premium per thousand if applicable.
  name: flatExtra
  type: number
- description: Any exclusions applied to the policy.
  name: exclusions
  type: array
- description: Reasons contributing to the underwriting decision.
  name: decisionReasons
  type: array
- description: Whether this decision was made fully automatically without human review.
  name: automatedDecision
  type: boolean
- description: If referred, the queue or team to which the case was referred.
  name: referralQueue
  type: string
- description: Details about the policy being underwritten.
  name: policyDetails
  type: object
- description: Version of the underwriting rule set used to make this decision.
  name: ruleSetVersion
  type: string
- description: Time in milliseconds taken to produce the decision.
  name: processingTimeMs
  type: integer
provider_name: Reinsurance Group of America
provider_slug: reinsurance-group-of-america
schema_file: json-schema/reinsurance-group-of-america-underwriting-decision-schema.json
slug: reinsurance-group-of-america-underwriting-decision
source_filename: reinsurance-group-of-america-underwriting-decision-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/reinsurance-group-of-america/json-schema/reinsurance-group-of-america-underwriting-decision-schema.json\",\n  \"title\": \"AURA NEXT Underwriting Decision\",\n  \"description\": \"Schema for an automated underwriting decision returned by RGA's AURA NEXT platform API.\",\n  \"type\": \"object\",\n  \"required\": [\"applicationId\", \"decisionDate\", \"decision\"],\n  \"properties\": {\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the insurance application.\"\n    },\n    \"decisionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this underwriting decision.\"\n    },\n    \"decisionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the underwriting decision was made.\"\n    },\n    \"decision\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"The underwriting decision outcome.\",\n      \"enum\": [\"Approved\", \"Approved with Modifications\", \"Referred\", \"Declined\", \"Postponed\", \"Pending Information\"]\n    },\n    \"riskClass\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned risk classification (e.g., 'Preferred Plus', 'Standard', 'Substandard').\"\n    },\n    \"tableRating\": {\n      \"type\": \"integer\",\n      \"description\": \"Table rating if applicable (percentage above standard mortality, in multiples of 25).\",\n      \"minimum\": 0\n    },\n    \"flatExtra\": {\n      \"type\": \"number\",\n      \"description\": \"Flat extra premium per thousand if applicable.\"\n    },\n    \"exclusions\": {\n      \"type\": \"array\",\n      \"items\": { \"type\": \"string\" },\n      \"description\": \"Any exclusions applied to the policy.\"\n    },\n    \"decisionReasons\": {\n      \"type\": \"array\",\n      \"description\": \"Reasons contributing to the\
  \ underwriting decision.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"reasonCode\": {\n            \"type\": \"string\",\n            \"description\": \"Coded reason for the decision factor.\"\n          },\n          \"reasonDescription\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable description of this decision factor.\"\n          },\n          \"weight\": {\n            \"type\": \"number\",\n            \"description\": \"Relative weight of this factor in the decision.\"\n          }\n        }\n      }\n    },\n    \"automatedDecision\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this decision was made fully automatically without human review.\"\n    },\n    \"referralQueue\": {\n      \"type\": \"string\",\n      \"description\": \"If referred, the queue or team to which the case was referred.\"\n    },\n    \"policyDetails\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Details about the policy being underwritten.\",\n      \"properties\": {\n        \"productType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of insurance product (e.g., 'Term Life', 'Universal Life', 'Whole Life').\"\n        },\n        \"faceAmount\": {\n          \"type\": \"number\",\n          \"description\": \"Face amount of coverage requested in dollars.\"\n        },\n        \"issueAge\": {\n          \"type\": \"integer\",\n          \"description\": \"Age of the applicant at policy issue.\"\n        },\n        \"gender\": {\n          \"type\": \"string\",\n          \"enum\": [\"Male\", \"Female\", \"Non-Binary\", \"Unknown\"]\n        }\n      }\n    },\n    \"ruleSetVersion\": {\n      \"type\": \"string\",\n      \"description\": \"Version of the underwriting rule set used to make this decision.\"\n    },\n    \"processingTimeMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Time in milliseconds taken to produce the decision.\"\
  \n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reinsurance-group-of-america/refs/heads/main/json-schema/reinsurance-group-of-america-underwriting-decision-schema.json
tags:
- Financial Services
- Health Insurance
- Insurance Technology
- Life Insurance
- Reinsurance
- Underwriting
title: AURA NEXT Underwriting Decision
---
