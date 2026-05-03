---
description: Schema for SAP S/4HANA Business Partner entity (A_BusinessPartner) from the API_BUSINESS_PARTNER OData service. Represents a business partner record which can be a Person (1), Organization (2), or Group (3).
layout: schema
name: SAP Business Partner
properties_list:
- description: Business partner number
  name: BusinessPartner
  type: string
- description: Business partner category (1=Person, 2=Organization, 3=Group)
  name: BusinessPartnerCategory
  type: string
- description: Full name of the business partner
  name: BusinessPartnerFullName
  type: string
- description: Business partner grouping
  name: BusinessPartnerGrouping
  type: string
- description: Business partner name
  name: BusinessPartnerName
  type: string
- description: First name (for person category)
  name: FirstName
  type: string
- description: Last name (for person category)
  name: LastName
  type: string
- description: Organization name line 1
  name: OrganizationBPName1
  type: string
- description: Organization name line 2
  name: OrganizationBPName2
  type: string
- description: Search term 1
  name: SearchTerm1
  type: string
- description: Language key
  name: Language
  type: string
- description: Date when the business partner was created
  name: CreationDate
  type: string
- description: Date of last change
  name: LastChangeDate
  type: string
- description: Central block flag
  name: BusinessPartnerIsBlocked
  type: boolean
- description: Natural person flag
  name: IsNaturalPerson
  type: string
- description: Trading partner company ID
  name: TradingPartner
  type: string
provider_name: SAP Sales and Distribution (SD)
provider_slug: sap-sales-and-distribution-sd
schema_file: json-schema/sap-sd-business-partner-schema.json
slug: sap-sd-business-partner
source_filename: sap-sd-business-partner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.sap.com/schemas/sap-sd-business-partner\",\n  \"title\": \"SAP Business Partner\",\n  \"description\": \"Schema for SAP S/4HANA Business Partner entity (A_BusinessPartner) from the API_BUSINESS_PARTNER OData service. Represents a business partner record which can be a Person (1), Organization (2), or Group (3).\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BusinessPartner\": {\n      \"type\": \"string\",\n      \"maxLength\": 10,\n      \"description\": \"Business partner number\"\n    },\n    \"BusinessPartnerCategory\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"enum\": [\"1\", \"2\", \"3\"],\n      \"description\": \"Business partner category (1=Person, 2=Organization, 3=Group)\"\n    },\n    \"BusinessPartnerFullName\": {\n      \"type\": \"string\",\n      \"maxLength\": 81,\n      \"description\": \"Full name of the business partner\"\n    },\n\
  \    \"BusinessPartnerGrouping\": {\n      \"type\": \"string\",\n      \"maxLength\": 4,\n      \"description\": \"Business partner grouping\"\n    },\n    \"BusinessPartnerName\": {\n      \"type\": \"string\",\n      \"maxLength\": 81,\n      \"description\": \"Business partner name\"\n    },\n    \"FirstName\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"First name (for person category)\"\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"Last name (for person category)\"\n    },\n    \"OrganizationBPName1\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"Organization name line 1\"\n    },\n    \"OrganizationBPName2\": {\n      \"type\": \"string\",\n      \"maxLength\": 40,\n      \"description\": \"Organization name line 2\"\n    },\n    \"SearchTerm1\": {\n      \"type\": \"string\",\n      \"maxLength\": 20,\n      \"description\": \"Search term\
  \ 1\"\n    },\n    \"Language\": {\n      \"type\": \"string\",\n      \"maxLength\": 2,\n      \"description\": \"Language key\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the business partner was created\"\n    },\n    \"LastChangeDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of last change\"\n    },\n    \"BusinessPartnerIsBlocked\": {\n      \"type\": \"boolean\",\n      \"description\": \"Central block flag\"\n    },\n    \"IsNaturalPerson\": {\n      \"type\": \"string\",\n      \"maxLength\": 1,\n      \"description\": \"Natural person flag\"\n    },\n    \"TradingPartner\": {\n      \"type\": \"string\",\n      \"maxLength\": 6,\n      \"description\": \"Trading partner company ID\"\n    }\n  },\n  \"required\": [\"BusinessPartner\", \"BusinessPartnerCategory\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-sales-and-distribution-sd/refs/heads/main/json-schema/sap-sd-business-partner-schema.json
tags:
- Distribution
- ERP
- OData
- S/4HANA
- Sales
- SAP
title: SAP Business Partner
---
