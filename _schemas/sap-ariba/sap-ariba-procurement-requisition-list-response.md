---
description: Paginated list of requisitions
layout: schema
name: RequisitionListResponse
properties_list:
- description: ''
  name: totalCount
  type: integer
- description: ''
  name: skip
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: requisitions
  type: array
provider_name: SAP Ariba
provider_slug: sap-ariba
schema_file: json-schema/sap-ariba-procurement-requisition-list-response-schema.json
slug: sap-ariba-procurement-requisition-list-response
source_filename: sap-ariba-procurement-requisition-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RequisitionListResponse\",\n  \"type\": \"object\",\n  \"description\": \"Paginated list of requisitions\",\n  \"properties\": {\n    \"totalCount\": {\n      \"type\": \"integer\"\n    },\n    \"skip\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"requisitions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-ariba/refs/heads/main/json-schema/sap-ariba-procurement-requisition-list-response-schema.json
tags:
- B2B
- Contract Management
- Procurement
- Sourcing
- Spend Analysis
- Supplier Management
- Supply Chain
title: RequisitionListResponse
---
