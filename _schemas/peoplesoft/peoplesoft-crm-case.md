---
description: PeopleSoft CRM service case.
layout: schema
name: Case
properties_list:
- description: Case ID.
  name: CASE_ID
  type: string
- description: Business unit.
  name: BUSINESS_UNIT
  type: string
- description: Customer ID.
  name: CUST_ID
  type: string
- description: Case description.
  name: DESCR
  type: string
- description: Priority.
  name: PRIORITY
  type: string
- description: Case status.
  name: STATUS
  type: string
- description: Case category.
  name: CATEGORY
  type: string
- description: Assigned agent.
  name: ASSIGNED_TO
  type: string
- description: Created date/time.
  name: CREATED_DTTM
  type: string
- description: Resolved date/time.
  name: RESOLVED_DTTM
  type: string
provider_name: PeopleSoft
provider_slug: peoplesoft
schema_file: json-schema/peoplesoft-crm-case-schema.json
slug: peoplesoft-crm-case
source_filename: peoplesoft-crm-case-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-crm-case-schema.json\",\n  \"title\": \"Case\",\n  \"description\": \"PeopleSoft CRM service case.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CASE_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Case ID.\",\n      \"example\": \"CASE001234\"\n    },\n    \"BUSINESS_UNIT\": {\n      \"type\": \"string\",\n      \"description\": \"Business unit.\",\n      \"example\": \"US001\"\n    },\n    \"CUST_ID\": {\n      \"type\": \"string\",\n      \"description\": \"Customer ID.\",\n      \"example\": \"CUST005678\"\n    },\n    \"DESCR\": {\n      \"type\": \"string\",\n      \"description\": \"Case description.\",\n      \"example\": \"Product defect inquiry\"\n    },\n    \"PRIORITY\": {\n      \"type\": \"string\",\n      \"description\": \"Priority.\",\n      \"enum\": [\n\
  \        \"1\",\n        \"2\",\n        \"3\",\n        \"4\"\n      ],\n      \"example\": \"2\"\n    },\n    \"STATUS\": {\n      \"type\": \"string\",\n      \"description\": \"Case status.\",\n      \"enum\": [\n        \"Open\",\n        \"In Progress\",\n        \"Resolved\",\n        \"Closed\"\n      ],\n      \"example\": \"Open\"\n    },\n    \"CATEGORY\": {\n      \"type\": \"string\",\n      \"description\": \"Case category.\",\n      \"example\": \"Product Support\"\n    },\n    \"ASSIGNED_TO\": {\n      \"type\": \"string\",\n      \"description\": \"Assigned agent.\",\n      \"example\": \"AGT001\"\n    },\n    \"CREATED_DTTM\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Created date/time.\",\n      \"example\": \"2026-04-17T09:30:00Z\"\n    },\n    \"RESOLVED_DTTM\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Resolved date/time.\"\n    }\n  },\n  \"x-schema-source\": \"domain-knowledge\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/peoplesoft/refs/heads/main/json-schema/peoplesoft-crm-case-schema.json
tags:
- Campus Solutions
- CRM
- Enterprise Software
- ERP
- Financial Management
- HCM
- Supply Chain Management
title: Case
---
