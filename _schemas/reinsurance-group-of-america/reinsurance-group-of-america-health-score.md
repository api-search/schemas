---
description: Schema for the risk score returned by RGA's Digital Health Data (DHD) scoring API based on structured electronic medical record and claims data.
layout: schema
name: Digital Health Data Risk Score
properties_list:
- description: Unique identifier for this scoring request.
  name: requestId
  type: string
- description: Identifier of the insurance application being scored.
  name: applicationId
  type: string
- description: Timestamp when the risk score was generated.
  name: scoreDate
  type: string
- description: Calculated risk score. Higher values indicate higher risk.
  name: riskScore
  type: number
- description: Risk category derived from the score.
  name: riskCategory
  type: string
- description: Confidence level of the score from 0.0 to 1.0.
  name: scoreConfidence
  type: number
- description: Summary of data sources available for scoring.
  name: dataAvailability
  type: object
- description: Key health signals that contributed to the risk score.
  name: healthSignals
  type: array
- description: Underwriting action recommendation based on the score.
  name: recommendation
  type: string
- description: Time in milliseconds to process and return the score.
  name: processingTimeMs
  type: integer
provider_name: Reinsurance Group of America
provider_slug: reinsurance-group-of-america
schema_file: json-schema/reinsurance-group-of-america-health-score-schema.json
slug: reinsurance-group-of-america-health-score
source_filename: reinsurance-group-of-america-health-score-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/reinsurance-group-of-america/json-schema/reinsurance-group-of-america-health-score-schema.json\",\n  \"title\": \"Digital Health Data Risk Score\",\n  \"description\": \"Schema for the risk score returned by RGA's Digital Health Data (DHD) scoring API based on structured electronic medical record and claims data.\",\n  \"type\": \"object\",\n  \"required\": [\"requestId\", \"applicationId\", \"scoreDate\", \"riskScore\"],\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this scoring request.\"\n    },\n    \"applicationId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the insurance application being scored.\"\n    },\n    \"scoreDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the risk score was generated.\"\
  \n    },\n    \"riskScore\": {\n      \"type\": \"number\",\n      \"description\": \"Calculated risk score. Higher values indicate higher risk.\",\n      \"minimum\": 0\n    },\n    \"riskCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Risk category derived from the score.\",\n      \"enum\": [\"Low Risk\", \"Moderate Risk\", \"High Risk\", \"Very High Risk\", \"Uninsurable\"]\n    },\n    \"scoreConfidence\": {\n      \"type\": \"number\",\n      \"description\": \"Confidence level of the score from 0.0 to 1.0.\",\n      \"minimum\": 0,\n      \"maximum\": 1\n    },\n    \"dataAvailability\": {\n      \"type\": \"object\",\n      \"description\": \"Summary of data sources available for scoring.\",\n      \"properties\": {\n        \"ehrDataAvailable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether electronic health record data was available.\"\n        },\n        \"claimsDataAvailable\": {\n          \"type\": \"boolean\",\n         \
  \ \"description\": \"Whether medical claims data was available.\"\n        },\n        \"rxDataAvailable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether prescription drug data was available.\"\n        },\n        \"labDataAvailable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether lab result data was available.\"\n        }\n      }\n    },\n    \"healthSignals\": {\n      \"type\": \"array\",\n      \"description\": \"Key health signals that contributed to the risk score.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"signalType\": {\n            \"type\": \"string\",\n            \"description\": \"Type of health signal (e.g., 'Diagnosis', 'Medication', 'Lab Result').\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Medical code (ICD-10, NDC, LOINC, etc.).\"\n          },\n          \"description\": {\n            \"type\": \"\
  string\",\n            \"description\": \"Human-readable description of the health signal.\"\n          },\n          \"riskContribution\": {\n            \"type\": \"number\",\n            \"description\": \"Contribution of this signal to the overall risk score.\"\n          }\n        }\n      }\n    },\n    \"recommendation\": {\n      \"type\": \"string\",\n      \"description\": \"Underwriting action recommendation based on the score.\",\n      \"enum\": [\"Straight Through Processing\", \"Accelerated Underwriting\", \"Refer for Review\", \"Order Additional Requirements\", \"Decline\"]\n    },\n    \"processingTimeMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Time in milliseconds to process and return the score.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reinsurance-group-of-america/refs/heads/main/json-schema/reinsurance-group-of-america-health-score-schema.json
tags:
- Financial Services
- Health Insurance
- Insurance Technology
- Life Insurance
- Reinsurance
- Underwriting
title: Digital Health Data Risk Score
---
