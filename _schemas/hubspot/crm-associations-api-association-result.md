---
description: Result of an association query
layout: schema
name: AssociationResult
properties_list:
- description: Reference to a CRM object by ID
  name: from
  type: object
- description: Associated objects
  name: to
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-associations-api-association-result-schema.json
slug: crm-associations-api-association-result
source_filename: crm-associations-api-association-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-association-result-schema.json\",\n  \"title\": \"AssociationResult\",\n  \"description\": \"Result of an association query\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"object\",\n      \"description\": \"Reference to a CRM object by ID\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the object\",\n          \"example\": \"500123\"\n        }\n      },\n      \"required\": [\n        \"id\"\n      ]\n    },\n    \"to\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents an association between two CRM objects\",\n        \"properties\": {\n          \"toObjectId\": {\n            \"type\": \"string\",\n            \"\
  description\": \"ID of the target object\",\n            \"example\": \"500123\"\n          },\n          \"associationTypes\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/AssociationType\"\n            },\n            \"description\": \"Types of associations between the objects\",\n            \"example\": [\n              {\n                \"associationCategory\": \"HUBSPOT_DEFINED\",\n                \"associationTypeId\": 500123,\n                \"label\": \"Example Record\"\n              }\n            ]\n          }\n        },\n        \"required\": [\n          \"toObjectId\",\n          \"associationTypes\"\n        ]\n      },\n      \"description\": \"Associated objects\",\n      \"example\": [\n        {\n          \"toObjectId\": \"500123\",\n          \"associationTypes\": [\n            {\n              \"associationCategory\": \"HUBSPOT_DEFINED\",\n              \"associationTypeId\": 500123,\n       \
  \       \"label\": \"Example Record\"\n            }\n          ]\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor for next page\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor token for the next page\",\n              \"example\": \"example-value\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the next page\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"from\",\n    \"to\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-association-result-schema.json
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
title: AssociationResult
---
