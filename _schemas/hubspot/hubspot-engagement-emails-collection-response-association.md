---
description: ''
layout: schema
name: CollectionResponseAssociation
properties_list:
- description: ''
  name: results
  type: array
- description: ''
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-emails-collection-response-association-schema.json
slug: hubspot-engagement-emails-collection-response-association
source_filename: hubspot-engagement-emails-collection-response-association-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"type\": \"standard\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          }\n        }\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"example\": {\n            \"after\": \"example-value\"\n          },\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CollectionResponseAssociation\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-emails-collection-response-association-schema.json
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
title: CollectionResponseAssociation
---
