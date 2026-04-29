---
description: JSON Schema for an Availity healthcare eligibility and benefits response (equivalent to X12 271 transaction).
layout: schema
name: Availity Eligibility Response
properties_list:
- description: Availity transaction identifier
  name: id
  type: string
- description: Transaction control number matching the request
  name: controlNumber
  type: string
- description: ''
  name: requestedDate
  type: string
- description: ''
  name: serviceDate
  type: string
- description: ''
  name: subscriber
  type: object
- description: ''
  name: payer
  type: object
- description: ''
  name: coverages
  type: array
- description: ''
  name: planInformation
  type: object
provider_name: availity
provider_slug: availity
schema_file: json-schema/availity-eligibility-schema.json
slug: availity-eligibility
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/availity-eligibility-schema.json\",\n  \"title\": \"Availity Eligibility Response\",\n  \"description\": \"JSON Schema for an Availity healthcare eligibility and benefits response (equivalent to X12 271 transaction).\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"subscriber\", \"payer\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Availity transaction identifier\"\n    },\n    \"controlNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Transaction control number matching the request\",\n      \"maxLength\": 9\n    },\n    \"requestedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"serviceDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\"\n    },\n    \"subscriber\": {\n      \"$ref\"\
  : \"#/$defs/SubscriberInfo\"\n    },\n    \"payer\": {\n      \"$ref\": \"#/$defs/PayerInfo\"\n    },\n    \"coverages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Coverage\"\n      }\n    },\n    \"planInformation\": {\n      \"$ref\": \"#/$defs/PlanInformation\"\n    }\n  },\n  \"$defs\": {\n    \"SubscriberInfo\": {\n      \"type\": \"object\",\n      \"required\": [\"memberId\"],\n      \"properties\": {\n        \"memberId\": {\"type\": \"string\"},\n        \"firstName\": {\"type\": \"string\"},\n        \"lastName\": {\"type\": \"string\"},\n        \"dateOfBirth\": {\"type\": \"string\", \"format\": \"date\"},\n        \"gender\": {\"type\": \"string\", \"enum\": [\"M\", \"F\", \"U\"]},\n        \"groupNumber\": {\"type\": \"string\"},\n        \"groupName\": {\"type\": \"string\"}\n      }\n    },\n    \"PayerInfo\": {\n      \"type\": \"object\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\"type\":\
  \ \"string\", \"description\": \"Availity payer ID\"},\n        \"name\": {\"type\": \"string\"}\n      }\n    },\n    \"Coverage\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"serviceTypeCodes\": {\n          \"type\": \"array\",\n          \"items\": {\"type\": \"string\"},\n          \"description\": \"X12 service type codes (e.g., 30=Health Benefit Plan, 1=Medical)\"\n        },\n        \"serviceTypeNames\": {\n          \"type\": \"array\",\n          \"items\": {\"type\": \"string\"}\n        },\n        \"coverageStatus\": {\n          \"type\": \"string\",\n          \"enum\": [\"Active\", \"Inactive\", \"Cancelled\"]\n        },\n        \"effectiveDate\": {\"type\": \"string\", \"format\": \"date\"},\n        \"expirationDate\": {\"type\": \"string\", \"format\": \"date\"},\n        \"benefits\": {\n          \"type\": \"array\",\n          \"items\": {\"$ref\": \"#/$defs/Benefit\"}\n        }\n      }\n    },\n    \"Benefit\": {\n      \"type\": \"object\"\
  ,\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"X12 benefit info code (e.g., 1=Active Coverage, C=Deductible, G=Co-payment)\"\n        },\n        \"name\": {\"type\": \"string\"},\n        \"coverageLevel\": {\n          \"type\": \"string\",\n          \"enum\": [\"INDIVIDUAL\", \"FAMILY\", \"EMPLOYEE\", \"EMPLOYEE_AND_SPOUSE\"]\n        },\n        \"benefitAmount\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\"type\": \"number\", \"minimum\": 0},\n            \"currency\": {\"type\": \"string\"}\n          }\n        },\n        \"benefitPercent\": {\n          \"type\": \"number\",\n          \"minimum\": 0,\n          \"maximum\": 100\n        },\n        \"inPlanNetworkIndicator\": {\n          \"type\": \"string\",\n          \"enum\": [\"Y\", \"N\", \"W\"],\n          \"description\": \"Y=In-network, N=Out-of-network, W=Not applicable\"\n        },\n        \"timeQualifier\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Benefit period qualifier\"\n        }\n      }\n    },\n    \"PlanInformation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"planName\": {\"type\": \"string\"},\n        \"groupName\": {\"type\": \"string\"},\n        \"groupNumber\": {\"type\": \"string\"},\n        \"planBeginDate\": {\"type\": \"string\", \"format\": \"date\"},\n        \"planEndDate\": {\"type\": \"string\", \"format\": \"date\"}\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/availity-eligibility-schema.json
tags: []
title: Availity Eligibility Response
---
