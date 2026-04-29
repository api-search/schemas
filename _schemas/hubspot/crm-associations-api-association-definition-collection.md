---
description: Collection of association definitions
layout: schema
name: AssociationDefinitionCollection
properties_list:
- description: Array of association definitions
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-associations-api-association-definition-collection-schema.json
slug: crm-associations-api-association-definition-collection
source_filename: crm-associations-api-association-definition-collection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-association-definition-collection-schema.json\",\n  \"title\": \"AssociationDefinitionCollection\",\n  \"description\": \"Collection of association definitions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Definition of an association type between two object types\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier for the association definition\",\n            \"example\": \"500123\"\n          },\n          \"fromObjectTypeId\": {\n            \"type\": \"string\",\n            \"description\": \"Source object type ID\",\n            \"example\": \"500123\"\n          },\n    \
  \      \"toObjectTypeId\": {\n            \"type\": \"string\",\n            \"description\": \"Target object type ID\",\n            \"example\": \"500123\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"Name of the association type\",\n            \"example\": \"Example Record\"\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"description\": \"Display label for the association\",\n            \"example\": \"Example Record\"\n          },\n          \"inverseLabel\": {\n            \"type\": \"string\",\n            \"description\": \"Label for the inverse association\",\n            \"example\": \"Example Record\"\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"HUBSPOT_DEFINED\",\n              \"USER_DEFINED\",\n              \"INTEGRATOR_DEFINED\"\n            ],\n            \"description\": \"Category of the association\
  \ definition\",\n            \"example\": \"HUBSPOT_DEFINED\"\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"fromObjectTypeId\",\n          \"toObjectTypeId\"\n        ]\n      },\n      \"description\": \"Array of association definitions\",\n      \"example\": [\n        {\n          \"id\": \"500123\",\n          \"fromObjectTypeId\": \"500123\",\n          \"toObjectTypeId\": \"500123\",\n          \"name\": \"Example Record\",\n          \"label\": \"Example Record\",\n          \"inverseLabel\": \"Example Record\",\n          \"category\": \"HUBSPOT_DEFINED\"\n        }\n      ]\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination cursor for next page\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"Cursor token for the next page\",\n              \"example\": \"example-value\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the next page\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-association-definition-collection-schema.json
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
title: AssociationDefinitionCollection
---
