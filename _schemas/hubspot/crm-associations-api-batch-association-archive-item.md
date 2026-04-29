---
description: Single item in a batch association archive request
layout: schema
name: BatchAssociationArchiveItem
properties_list:
- description: Reference to a CRM object by ID
  name: from
  type: object
- description: Reference to a CRM object by ID
  name: to
  type: object
- description: ''
  name: types
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-associations-api-batch-association-archive-item-schema.json
slug: crm-associations-api-batch-association-archive-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-archive-item-schema.json\",\n  \"title\": \"BatchAssociationArchiveItem\",\n  \"description\": \"Single item in a batch association archive request\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a CRM object by ID\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the object\",\n          \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"to\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a CRM object by ID\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the object\",\n     \
  \     \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"types\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Input for specifying an association type\",\n        \"properties\": {\n          \"associationCategory\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HUBSPOT_DEFINED\",\n              \"USER_DEFINED\",\n              \"INTEGRATOR_DEFINED\"\n            ],\n            \"example\": \"HUBSPOT_DEFINED\"\n          },\n          \"associationTypeId\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          }\n        },\n        \"required\": [\n          \"associationCategory\",\n          \"associationTypeId\"\n        ]\n      },\n      \"example\": [\n        {\n          \"associationCategory\": \"HUBSPOT_DEFINED\",\n          \"associationTypeId\": 500123\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"from\",\n    \"to\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-archive-item-schema.json
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
title: BatchAssociationArchiveItem
---
