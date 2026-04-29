---
description: ''
layout: schema
name: BusinessPartnerRole
properties_list:
- description: Business partner number
  name: BusinessPartner
  type: string
- description: Role code (e.g., FLCU01=Customer, FLVN01=Vendor)
  name: BusinessPartnerRole
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-s4hana-cloud-business-partner-business-partner-role-schema.json
slug: sap-s4hana-cloud-business-partner-business-partner-role
source_filename: sap-s4hana-cloud-business-partner-business-partner-role-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BusinessPartnerRole\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BusinessPartner\": {\n      \"type\": \"string\",\n      \"description\": \"Business partner number\"\n    },\n    \"BusinessPartnerRole\": {\n      \"type\": \"string\",\n      \"description\": \"Role code (e.g., FLCU01=Customer, FLVN01=Vendor)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-s4hana-cloud-business-partner-business-partner-role-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: BusinessPartnerRole
---
