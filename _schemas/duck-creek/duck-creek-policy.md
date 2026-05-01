---
description: Schema representing a P&C insurance policy managed in Duck Creek Policy Administration.
layout: schema
name: Duck Creek Insurance Policy
properties_list:
- description: Internal Duck Creek policy identifier
  name: policyId
  type: string
- description: Human-readable policy number
  name: policyNumber
  type: string
- description: Current policy lifecycle status
  name: status
  type: string
- description: Duck Creek product code identifying the insurance product
  name: productCode
  type: string
- description: Insurance line of business
  name: lineOfBusiness
  type: string
- description: Policy effective date
  name: effectiveDate
  type: string
- description: Policy expiration date
  name: expirationDate
  type: string
- description: ''
  name: insured
  type: object
- description: List of coverages included in the policy
  name: coverages
  type: array
- description: Total annualized premium in USD
  name: totalPremium
  type: number
- description: Insurance company writing the policy
  name: writingCompany
  type: string
- description: Producing agent code
  name: agentCode
  type: string
- description: Associated billing account identifier
  name: billingAccountId
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: duck-creek
provider_slug: duck-creek
schema_file: json-schema/duck-creek-policy-schema.json
slug: duck-creek-policy
source_filename: duck-creek-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.duckcreek.com/v1/schemas/policy\",\n  \"title\": \"Duck Creek Insurance Policy\",\n  \"description\": \"Schema representing a P&C insurance policy managed in Duck Creek Policy Administration.\",\n  \"type\": \"object\",\n  \"required\": [\"policyId\", \"policyNumber\", \"status\", \"productCode\", \"insured\", \"effectiveDate\"],\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Internal Duck Creek policy identifier\",\n      \"format\": \"uuid\"\n    },\n    \"policyNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable policy number\",\n      \"examples\": [\"PA-2026-001234\", \"HO-2026-567890\"]\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current policy lifecycle status\",\n      \"enum\": [\"QUOTED\", \"IN_FORCE\", \"CANCELLED\", \"EXPIRED\", \"PENDING_CANCEL\", \"RENEWAL\"\
  , \"RESCINDED\"]\n    },\n    \"productCode\": {\n      \"type\": \"string\",\n      \"description\": \"Duck Creek product code identifying the insurance product\"\n    },\n    \"lineOfBusiness\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance line of business\",\n      \"enum\": [\"AUTO\", \"HOME\", \"COMMERCIAL_PROPERTY\", \"GENERAL_LIABILITY\", \"WORKERS_COMP\", \"UMBRELLA\", \"SPECIALTY\"]\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy effective date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy expiration date\"\n    },\n    \"insured\": {\n      \"$ref\": \"#/$defs/Insured\"\n    },\n    \"coverages\": {\n      \"type\": \"array\",\n      \"description\": \"List of coverages included in the policy\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Coverage\"\n      }\n    },\n    \"totalPremium\": {\n\
  \      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Total annualized premium in USD\",\n      \"minimum\": 0\n    },\n    \"writingCompany\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance company writing the policy\"\n    },\n    \"agentCode\": {\n      \"type\": \"string\",\n      \"description\": \"Producing agent code\"\n    },\n    \"billingAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated billing account identifier\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Insured\": {\n      \"type\": \"object\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the insured\"\n        },\n        \"type\": {\n          \"type\": \"\
  string\",\n          \"enum\": [\"INDIVIDUAL\", \"BUSINESS\"]\n        },\n        \"dateOfBirth\": {\n          \"type\": \"string\",\n          \"format\": \"date\",\n          \"description\": \"Insured date of birth (for individual policyholders)\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        },\n        \"phone\": {\n          \"type\": \"string\"\n        },\n        \"email\": {\n          \"type\": \"string\",\n          \"format\": \"email\"\n        }\n      }\n    },\n    \"Coverage\": {\n      \"type\": \"object\",\n      \"required\": [\"coverageCode\"],\n      \"properties\": {\n        \"coverageCode\": {\n          \"type\": \"string\",\n          \"description\": \"Duck Creek coverage type code\",\n          \"examples\": [\"BI\", \"PD\", \"COMP\", \"COLL\", \"DWELLING\", \"LIABILITY\"]\n        },\n        \"coverageName\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable coverage name\"\n       \
  \ },\n        \"limit\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Coverage limit in USD\",\n          \"minimum\": 0\n        },\n        \"deductible\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Coverage deductible in USD\",\n          \"minimum\": 0\n        },\n        \"premium\": {\n          \"type\": \"number\",\n          \"format\": \"double\",\n          \"description\": \"Coverage premium contribution in USD\",\n          \"minimum\": 0\n        },\n        \"subLimits\": {\n          \"type\": \"array\",\n          \"description\": \"Sub-limits within this coverage\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"subLimitCode\": { \"type\": \"string\" },\n              \"amount\": { \"type\": \"number\" }\n            }\n          }\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"\
  object\",\n      \"properties\": {\n        \"street1\": { \"type\": \"string\" },\n        \"street2\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n        \"state\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\",\n          \"description\": \"US state code\"\n        },\n        \"zipCode\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[0-9]{5}(-[0-9]{4})?$\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"default\": \"US\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/duck-creek/refs/heads/main/json-schema/duck-creek-policy-schema.json
tags: []
title: Duck Creek Insurance Policy
---
