---
description: Collection of association labels
layout: schema
name: AssociationLabelCollection
properties_list:
- description: Array of association labels
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-association-label-collection-schema.json
slug: hubspot-crm-associations-association-label-collection
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Collection of association labels\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of association labels\",\n      \"example\": [\n        {\n          \"typeId\": 500123,\n          \"label\": \"Example Record\",\n          \"category\": \"HUBSPOT_DEFINED\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A label that can be applied to associations\",\n        \"properties\": {\n          \"typeId\": {\n            \"type\": \"integer\",\n            \"description\": \"Numeric identifier for the label type\",\n            \"example\": 500123\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"Display text for the label\",\n            \"example\": \"Example Record\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"description\"\
  : \"Category of the label\",\n            \"example\": \"HUBSPOT_DEFINED\",\n            \"enum\": [\n              \"HUBSPOT_DEFINED\",\n              \"USER_DEFINED\",\n              \"INTEGRATOR_DEFINED\"\n            ]\n          }\n        },\n        \"required\": [\n          \"typeId\",\n          \"label\",\n          \"category\"\n        ]\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor for next page\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor token for the next page\",\n              \"example\": \"example-value\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the next page\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\
  \n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AssociationLabelCollection\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-association-label-collection-schema.json
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
title: AssociationLabelCollection
---
