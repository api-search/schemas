---
description: Represents a commercial real estate lease agreement in the ARGUS Enterprise platform, including tenant details, rent schedules, escalation terms, and lease options.
layout: schema
name: Argus Enterprise Lease
properties_list:
- description: Unique lease identifier
  name: id
  type: string
- description: Associated property identifier
  name: propertyId
  type: string
- description: Associated tenant identifier
  name: tenantId
  type: string
- description: Tenant name
  name: tenantName
  type: string
- description: Unit or suite number
  name: unitNumber
  type: string
- description: Type of lease
  name: leaseType
  type: string
- description: Current lease status
  name: status
  type: string
- description: Lease commencement date
  name: startDate
  type: string
- description: Lease expiration date
  name: endDate
  type: string
- description: Leased area in square feet
  name: leasedArea
  type: number
- description: Base rent amount per period
  name: baseRent
  type: number
- description: Rent payment frequency
  name: rentFrequency
  type: string
- description: Rent per square foot per annum
  name: rentPerSquareFoot
  type: number
- description: Annual rent escalation rate (percentage)
  name: escalationRate
  type: number
- description: Type of rent escalation
  name: escalationType
  type: string
- description: Security deposit amount
  name: securityDeposit
  type: number
- description: Tenant improvement allowance
  name: tenantImprovementAllowance
  type: number
- description: Lease renewal or expansion options
  name: options
  type: array
- description: Currency code (ISO 4217)
  name: currency
  type: string
- description: Record creation timestamp
  name: createdAt
  type: string
- description: Record last update timestamp
  name: updatedAt
  type: string
provider_name: ARGUS Enterprise
provider_slug: argus-enterprise
schema_file: json-schema/argus-enterprise-lease-schema.json
slug: argus-enterprise-lease
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.argusenterprise.com/schemas/argus-enterprise/lease.json\",\n  \"title\": \"Argus Enterprise Lease\",\n  \"description\": \"Represents a commercial real estate lease agreement in the ARGUS Enterprise platform, including tenant details, rent schedules, escalation terms, and lease options.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique lease identifier\"\n    },\n    \"propertyId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Associated property identifier\"\n    },\n    \"tenantId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Associated tenant identifier\"\n    },\n    \"tenantName\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant name\"\n    },\n    \"unitNumber\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Unit or suite number\"\n    },\n    \"leaseType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Gross\", \"Net\", \"DoubleNet\", \"TripleNet\", \"ModifiedGross\", \"PercentageRent\"],\n      \"description\": \"Type of lease\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Active\", \"Expired\", \"Pending\"],\n      \"description\": \"Current lease status\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Lease commencement date\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Lease expiration date\"\n    },\n    \"leasedArea\": {\n      \"type\": \"number\",\n      \"description\": \"Leased area in square feet\"\n    },\n    \"baseRent\": {\n      \"type\": \"number\",\n      \"description\": \"Base rent amount per period\"\n    },\n    \"rentFrequency\": {\n      \"type\": \"string\"\
  ,\n      \"enum\": [\"Monthly\", \"Quarterly\", \"Annual\"],\n      \"description\": \"Rent payment frequency\"\n    },\n    \"rentPerSquareFoot\": {\n      \"type\": \"number\",\n      \"description\": \"Rent per square foot per annum\"\n    },\n    \"escalationRate\": {\n      \"type\": \"number\",\n      \"description\": \"Annual rent escalation rate (percentage)\"\n    },\n    \"escalationType\": {\n      \"type\": \"string\",\n      \"enum\": [\"Fixed\", \"CPI\", \"MarketReset\", \"StepUp\"],\n      \"description\": \"Type of rent escalation\"\n    },\n    \"securityDeposit\": {\n      \"type\": \"number\",\n      \"description\": \"Security deposit amount\"\n    },\n    \"tenantImprovementAllowance\": {\n      \"type\": \"number\",\n      \"description\": \"Tenant improvement allowance\"\n    },\n    \"options\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"optionType\": {\n            \"type\": \"string\"\
  ,\n            \"enum\": [\"Renewal\", \"Expansion\", \"Termination\", \"PurchaseOption\"],\n            \"description\": \"Type of lease option\"\n          },\n          \"noticeDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\",\n            \"description\": \"Date by which notice must be given\"\n          },\n          \"exerciseDate\": {\n            \"type\": \"string\",\n            \"format\": \"date\",\n            \"description\": \"Date the option can be exercised\"\n          },\n          \"termMonths\": {\n            \"type\": \"integer\",\n            \"description\": \"Duration of option term in months\"\n          },\n          \"rentAdjustment\": {\n            \"type\": \"string\",\n            \"description\": \"Description of rent adjustment terms\"\n          }\n        }\n      },\n      \"description\": \"Lease renewal or expansion options\"\n    },\n    \"currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency\
  \ code (ISO 4217)\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record last update timestamp\"\n    }\n  },\n  \"required\": [\"tenantId\", \"leaseType\", \"startDate\", \"endDate\", \"baseRent\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/argus-enterprise/refs/heads/main/json-schema/argus-enterprise-lease-schema.json
tags:
- Altus Group
- Asset Management
- Cash Flow Modeling
- Commercial Real Estate
- Portfolio Management
- Valuation
title: Argus Enterprise Lease
---
