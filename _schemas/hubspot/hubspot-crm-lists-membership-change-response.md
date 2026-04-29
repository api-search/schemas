---
description: Response from a list membership change operation.
layout: schema
name: MembershipChangeResponse
properties_list:
- description: ''
  name: recordIdsAdded
  type: array
- description: ''
  name: recordIdsAlreadyMember
  type: array
- description: ''
  name: recordIdsRemoved
  type: array
- description: ''
  name: recordIdsMissing
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-lists-membership-change-response-schema.json
slug: hubspot-crm-lists-membership-change-response
source_filename: hubspot-crm-lists-membership-change-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Response from a list membership change operation.\",\n  \"properties\": {\n    \"recordIdsAdded\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"500123\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"recordIdsAlreadyMember\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"500123\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"recordIdsRemoved\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"500123\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"recordIdsMissing\": {\n      \"type\": \"array\",\n      \"example\": [\n        \"500123\"\n      ],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MembershipChangeResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-lists-membership-change-response-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: MembershipChangeResponse
---
