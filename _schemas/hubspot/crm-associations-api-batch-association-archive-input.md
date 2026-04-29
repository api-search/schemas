---
description: Input for batch archiving associations
layout: schema
name: BatchAssociationArchiveInput
properties_list:
- description: Associations to archive
  name: inputs
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/crm-associations-api-batch-association-archive-input-schema.json
slug: crm-associations-api-batch-association-archive-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-archive-input-schema.json\",\n  \"title\": \"BatchAssociationArchiveInput\",\n  \"description\": \"Input for batch archiving associations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"inputs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Single item in a batch association archive request\",\n        \"properties\": {\n          \"from\": {\n            \"$ref\": \"#/components/schemas/ObjectReference\"\n          },\n          \"to\": {\n            \"$ref\": \"#/components/schemas/ObjectReference\"\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"$ref\": \"#/components/schemas/AssociationTypeInput\"\n            },\n            \"example\"\
  : [\n              {\n                \"associationCategory\": \"HUBSPOT_DEFINED\",\n                \"associationTypeId\": 500123\n              }\n            ]\n          }\n        },\n        \"required\": [\n          \"from\",\n          \"to\"\n        ]\n      },\n      \"description\": \"Associations to archive\",\n      \"example\": [\n        {\n          \"from\": {},\n          \"to\": {},\n          \"types\": [\n            {}\n          ]\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"inputs\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/crm-associations-api-batch-association-archive-input-schema.json
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
title: BatchAssociationArchiveInput
---
