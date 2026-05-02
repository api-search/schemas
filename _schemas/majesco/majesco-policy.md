---
description: An insurance policy managed through the Majesco cloud platform
layout: schema
name: Majesco Insurance Policy
properties_list:
- description: Unique policy identifier
  name: policyNumber
  type: string
- description: Current lifecycle status of the policy
  name: status
  type: string
- description: Line of business / insurance product type
  name: productType
  type: string
- description: Policy inception date
  name: effectiveDate
  type: string
- description: Policy expiration date
  name: expirationDate
  type: string
- description: ''
  name: cancellationDate
  type:
  - string
  - 'null'
- description: ''
  name: policyholder
  type: object
- description: ''
  name: coverages
  type: array
- description: ''
  name: premium
  type: object
- description: ''
  name: endorsements
  type: array
- description: Issuing agent or broker code
  name: agentCode
  type: string
- description: Distribution channel identifier
  name: channelCode
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: majesco
provider_slug: majesco
schema_file: json-schema/majesco-policy-schema.json
slug: majesco-policy
source_filename: majesco-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/majesco/refs/heads/main/json-schema/majesco-policy-schema.json\",\n  \"title\": \"Majesco Insurance Policy\",\n  \"description\": \"An insurance policy managed through the Majesco cloud platform\",\n  \"type\": \"object\",\n  \"required\": [\"policyNumber\", \"productType\", \"effectiveDate\", \"expirationDate\", \"status\", \"policyholder\"],\n  \"properties\": {\n    \"policyNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Unique policy identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"active\", \"expired\", \"cancelled\", \"pending\", \"lapsed\"],\n      \"description\": \"Current lifecycle status of the policy\"\n    },\n    \"productType\": {\n      \"type\": \"string\",\n      \"enum\": [\"auto\", \"home\", \"commercial\", \"life\", \"health\", \"specialty\"],\n      \"description\"\
  : \"Line of business / insurance product type\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy inception date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy expiration date\"\n    },\n    \"cancellationDate\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date\"\n    },\n    \"policyholder\": {\n      \"$ref\": \"#/$defs/Policyholder\"\n    },\n    \"coverages\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Coverage\" }\n    },\n    \"premium\": {\n      \"$ref\": \"#/$defs/Premium\"\n    },\n    \"endorsements\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/Endorsement\" }\n    },\n    \"agentCode\": {\n      \"type\": \"string\",\n      \"description\": \"Issuing agent or broker code\"\n    },\n    \"channelCode\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Distribution channel identifier\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Policyholder\": {\n      \"type\": \"object\",\n      \"required\": [\"firstName\", \"lastName\"],\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"firstName\": { \"type\": \"string\" },\n        \"lastName\": { \"type\": \"string\" },\n        \"dateOfBirth\": { \"type\": \"string\", \"format\": \"date\" },\n        \"email\": { \"type\": \"string\", \"format\": \"email\" },\n        \"phone\": { \"type\": \"string\" },\n        \"address\": { \"$ref\": \"#/$defs/Address\" }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street1\": { \"type\": \"string\" },\n        \"street2\": { \"type\": \"string\" },\n        \"city\": { \"type\": \"string\" },\n\
  \        \"state\": { \"type\": \"string\", \"pattern\": \"^[A-Z]{2}$\" },\n        \"postalCode\": { \"type\": \"string\" },\n        \"country\": { \"type\": \"string\", \"default\": \"US\" }\n      }\n    },\n    \"Coverage\": {\n      \"type\": \"object\",\n      \"required\": [\"coverageCode\"],\n      \"properties\": {\n        \"coverageCode\": { \"type\": \"string\" },\n        \"coverageDescription\": { \"type\": \"string\" },\n        \"limit\": { \"type\": \"number\", \"minimum\": 0 },\n        \"deductible\": { \"type\": \"number\", \"minimum\": 0 },\n        \"premium\": { \"type\": \"number\", \"minimum\": 0 },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\"active\", \"excluded\", \"suspended\"]\n        }\n      }\n    },\n    \"Premium\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"annualPremium\": { \"type\": \"number\", \"minimum\": 0 },\n        \"taxAmount\": { \"type\": \"number\", \"minimum\": 0 },\n        \"\
  feesAmount\": { \"type\": \"number\", \"minimum\": 0 },\n        \"totalPremium\": { \"type\": \"number\", \"minimum\": 0 },\n        \"currency\": { \"type\": \"string\", \"default\": \"USD\" },\n        \"billingFrequency\": {\n          \"type\": \"string\",\n          \"enum\": [\"annual\", \"semi_annual\", \"quarterly\", \"monthly\"]\n        }\n      }\n    },\n    \"Endorsement\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"endorsementNumber\": { \"type\": \"string\" },\n        \"type\": { \"type\": \"string\" },\n        \"effectiveDate\": { \"type\": \"string\", \"format\": \"date\" },\n        \"description\": { \"type\": \"string\" },\n        \"premiumChange\": { \"type\": \"number\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/majesco/refs/heads/main/json-schema/majesco-policy-schema.json
tags: []
title: Majesco Insurance Policy
---
