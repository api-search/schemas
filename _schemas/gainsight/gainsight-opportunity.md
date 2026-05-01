---
description: Represents an opportunity record in the Gainsight Renewal Center, tracking renewals, upsells, downsells, and new business within the Matrix Data Architecture.
layout: schema
name: Gainsight Opportunity
properties_list:
- description: Opportunity unique identifier
  name: Gsid
  type: string
- description: Opportunity name
  name: Name
  type: string
- description: Associated company Gsid
  name: CompanyId
  type: string
- description: Associated company name
  name: CompanyName
  type: string
- description: Type of booking
  name: BookingType
  type: string
- description: Opportunity amount
  name: Amount
  type: number
- description: Currency code (e.g., USD, EUR)
  name: Currency
  type: string
- description: Expected or actual close date
  name: CloseDate
  type: string
- description: Opportunity stage
  name: Stage
  type: string
- description: Win probability percentage
  name: Probability
  type: number
- description: Opportunity owner user ID
  name: OwnerId
  type: string
- description: Owner display name
  name: OwnerName
  type: string
- description: Annual recurring revenue
  name: ARR
  type: number
- description: Contract term in months
  name: Term
  type: integer
- description: Renewal date
  name: RenewalDate
  type: string
- description: Whether the opportunity is closed
  name: IsClosed
  type: boolean
- description: Whether the opportunity was won
  name: IsWon
  type: boolean
- description: Linked Salesforce opportunity ID
  name: SfdcOpportunityId
  type: string
- description: Record creation timestamp
  name: CreatedDate
  type: string
- description: Record last modification timestamp
  name: ModifiedDate
  type: string
provider_name: Gainsight
provider_slug: gainsight
schema_file: json-schema/gainsight-opportunity-schema.json
slug: gainsight-opportunity
source_filename: gainsight-opportunity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://www.gainsight.com/schemas/gainsight/opportunity.json\",\n  \"title\": \"Gainsight Opportunity\",\n  \"description\": \"Represents an opportunity record in the Gainsight Renewal Center, tracking renewals, upsells, downsells, and new business within the Matrix Data Architecture.\",\n  \"type\": \"object\",\n  \"required\": [\"Name\", \"CompanyId\", \"BookingType\"],\n  \"properties\": {\n    \"Gsid\": {\n      \"type\": \"string\",\n      \"description\": \"Opportunity unique identifier\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"Opportunity name\"\n    },\n    \"CompanyId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company Gsid\"\n    },\n    \"CompanyName\": {\n      \"type\": \"string\",\n      \"description\": \"Associated company name\"\n    },\n    \"BookingType\": {\n      \"type\": \"string\",\n      \"enum\": [\"New\
  \ Business\", \"Renewal\", \"Upsell\", \"Downsell\", \"Churn\"],\n      \"description\": \"Type of booking\"\n    },\n    \"Amount\": {\n      \"type\": \"number\",\n      \"description\": \"Opportunity amount\",\n      \"minimum\": 0\n    },\n    \"Currency\": {\n      \"type\": \"string\",\n      \"description\": \"Currency code (e.g., USD, EUR)\"\n    },\n    \"CloseDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Expected or actual close date\"\n    },\n    \"Stage\": {\n      \"type\": \"string\",\n      \"description\": \"Opportunity stage\"\n    },\n    \"Probability\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Win probability percentage\"\n    },\n    \"OwnerId\": {\n      \"type\": \"string\",\n      \"description\": \"Opportunity owner user ID\"\n    },\n    \"OwnerName\": {\n      \"type\": \"string\",\n      \"description\": \"Owner display name\"\n    },\n    \"ARR\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Annual recurring revenue\",\n      \"minimum\": 0\n    },\n    \"Term\": {\n      \"type\": \"integer\",\n      \"description\": \"Contract term in months\",\n      \"minimum\": 1\n    },\n    \"RenewalDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Renewal date\"\n    },\n    \"IsClosed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the opportunity is closed\"\n    },\n    \"IsWon\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the opportunity was won\"\n    },\n    \"SfdcOpportunityId\": {\n      \"type\": \"string\",\n      \"description\": \"Linked Salesforce opportunity ID\"\n    },\n    \"CreatedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Record creation timestamp\"\n    },\n    \"ModifiedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Record last modification timestamp\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gainsight/refs/heads/main/json-schema/gainsight-opportunity-schema.json
tags: []
title: Gainsight Opportunity
---
