---
description: JSON Schema for an ACORD NGDS insurance policy object, representing an insurance contract with coverages and insured party.
layout: schema
name: ACORD Policy
properties_list:
- description: Unique internal policy identifier
  name: policyId
  type: string
- description: Carrier-assigned policy number
  name: policyNumber
  type: string
- description: Insurance line of business
  name: lineOfBusiness
  type: string
- description: Current policy status
  name: status
  type: string
- description: Policy effective date
  name: effectiveDate
  type: string
- description: Policy expiration date
  name: expirationDate
  type: string
- description: Total policy premium amount
  name: premiumAmount
  type: number
- description: ISO 4217 currency code
  name: currency
  type: string
- description: ''
  name: insuredParty
  type: object
- description: List of coverages under the policy
  name: coverages
  type: array
- description: Policy endorsements and amendments
  name: endorsements
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: ACORD
provider_slug: acord
schema_file: json-schema/acord-policy-schema.json
slug: acord-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/acord-policy-schema.json\",\n  \"title\": \"ACORD Policy\",\n  \"description\": \"JSON Schema for an ACORD NGDS insurance policy object, representing an insurance contract with coverages and insured party.\",\n  \"type\": \"object\",\n  \"required\": [\"policyId\", \"policyNumber\", \"lineOfBusiness\", \"status\", \"effectiveDate\", \"expirationDate\"],\n  \"properties\": {\n    \"policyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique internal policy identifier\"\n    },\n    \"policyNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Carrier-assigned policy number\"\n    },\n    \"lineOfBusiness\": {\n      \"type\": \"string\",\n      \"description\": \"Insurance line of business\",\n      \"enum\": [\"PropertyCasualty\", \"Life\", \"Annuity\", \"Reinsurance\"]\n    },\n   \
  \ \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current policy status\",\n      \"enum\": [\"Active\", \"Lapsed\", \"Cancelled\", \"Pending\", \"Expired\"]\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy effective date\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Policy expiration date\"\n    },\n    \"premiumAmount\": {\n      \"type\": \"number\",\n      \"description\": \"Total policy premium amount\",\n      \"minimum\": 0\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 4217 currency code\",\n      \"default\": \"USD\",\n      \"pattern\": \"^[A-Z]{3}$\"\n    },\n    \"insuredParty\": {\n      \"$ref\": \"#/$defs/Party\"\n    },\n    \"coverages\": {\n      \"type\": \"array\",\n      \"description\": \"List of coverages under the policy\",\n      \"items\": {\n       \
  \ \"$ref\": \"#/$defs/Coverage\"\n      }\n    },\n    \"endorsements\": {\n      \"type\": \"array\",\n      \"description\": \"Policy endorsements and amendments\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Endorsement\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"$defs\": {\n    \"Party\": {\n      \"type\": \"object\",\n      \"description\": \"ACORD NGDS Party representing an insured, claimant, agent, or broker\",\n      \"required\": [\"partyId\", \"partyType\"],\n      \"properties\": {\n        \"partyId\": {\n          \"type\": \"string\"\n        },\n        \"partyType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Insured\", \"Claimant\", \"Agent\", \"Broker\", \"Carrier\"]\n        },\n        \"firstName\": {\n          \"type\": \"string\"\n        },\n        \"lastName\": {\n      \
  \    \"type\": \"string\"\n        },\n        \"organizationName\": {\n          \"type\": \"string\"\n        },\n        \"taxId\": {\n          \"type\": \"string\",\n          \"description\": \"Tax identification number (SSN or EIN)\"\n        },\n        \"address\": {\n          \"$ref\": \"#/$defs/Address\"\n        },\n        \"contacts\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Contact\"\n          }\n        }\n      }\n    },\n    \"Coverage\": {\n      \"type\": \"object\",\n      \"description\": \"Insurance coverage detail\",\n      \"required\": [\"coverageId\", \"coverageType\"],\n      \"properties\": {\n        \"coverageId\": {\n          \"type\": \"string\"\n        },\n        \"coverageType\": {\n          \"type\": \"string\",\n          \"description\": \"Type of coverage (e.g., BodilyInjury, PropertyDamage, Medical)\"\n        },\n        \"limit\": {\n          \"type\": \"number\",\n          \"minimum\"\
  : 0\n        },\n        \"deductible\": {\n          \"type\": \"number\",\n          \"minimum\": 0\n        },\n        \"premium\": {\n          \"type\": \"number\",\n          \"minimum\": 0\n        },\n        \"currency\": {\n          \"type\": \"string\",\n          \"default\": \"USD\"\n        }\n      }\n    },\n    \"Endorsement\": {\n      \"type\": \"object\",\n      \"description\": \"Policy endorsement or amendment\",\n      \"required\": [\"endorsementNumber\", \"effectiveDate\"],\n      \"properties\": {\n        \"endorsementNumber\": {\n          \"type\": \"string\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"effectiveDate\": {\n          \"type\": \"string\",\n          \"format\": \"date\"\n        },\n        \"premiumChange\": {\n          \"type\": \"number\"\n        }\n      }\n    },\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"street1\": {\n          \"type\": \"\
  string\"\n        },\n        \"street2\": {\n          \"type\": \"string\"\n        },\n        \"city\": {\n          \"type\": \"string\"\n        },\n        \"state\": {\n          \"type\": \"string\",\n          \"pattern\": \"^[A-Z]{2}$\"\n        },\n        \"postalCode\": {\n          \"type\": \"string\"\n        },\n        \"country\": {\n          \"type\": \"string\",\n          \"default\": \"US\"\n        }\n      }\n    },\n    \"Contact\": {\n      \"type\": \"object\",\n      \"required\": [\"contactType\", \"value\"],\n      \"properties\": {\n        \"contactType\": {\n          \"type\": \"string\",\n          \"enum\": [\"Phone\", \"Email\", \"Fax\"]\n        },\n        \"value\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acord/refs/heads/main/json-schema/acord-policy-schema.json
tags:
- Claims
- Insurance
- Policy
- Standards
- Underwriting
title: ACORD Policy
---
