---
description: ''
layout: schema
name: BusinessPartner
properties_list:
- description: Business partner number
  name: BusinessPartner
  type: string
- description: Full name of the business partner
  name: BusinessPartnerFullName
  type: string
- description: Category (1=Organization, 2=Person, 3=Group)
  name: BusinessPartnerCategory
  type: string
- description: Business partner grouping
  name: BusinessPartnerGrouping
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
- description: Search term 1
  name: SearchTerm1
  type: string
- description: Correspondence language
  name: Language
  type: string
- description: Date the business partner was created
  name: CreationDate
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-s4hana-cloud-business-partner-business-partner-schema.json
slug: sap-s4hana-cloud-business-partner-business-partner
source_filename: sap-s4hana-cloud-business-partner-business-partner-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessPartner\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BusinessPartner\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner number\"\n    },\n    \"BusinessPartnerFullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full name of the business partner\"\n    },\n    \"BusinessPartnerCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Category (1=Organization, 2=Person, 3=Group)\"\n    },\n    \"BusinessPartnerGrouping\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner grouping\"\n    },\n    \"FirstName\": {\n      \"type\": \"string\",\n      \"description\": \"First name (for person category)\"\n    },\n    \"LastName\": {\n      \"type\": \"string\",\n      \"description\": \"Last name (for person category)\"\n    },\n    \"OrganizationBPName1\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Organization name line 1\"\n    },\n    \"SearchTerm1\": {\n      \"type\": \"string\",\n      \"description\": \"Search term 1\"\n    },\n    \"Language\": {\n      \"type\": \"string\",\n      \"description\": \"Correspondence language\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"description\": \"Date the business partner was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-s4hana-cloud-business-partner-business-partner-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: BusinessPartner
---
