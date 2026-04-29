---
description: A paginated collection of SMTP tokens
layout: schema
name: SmtpTokenCollectionResponse
properties_list:
- description: The list of SMTP tokens
  name: results
  type: array
- description: Pagination information
  name: paging
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-marketing-emal-smtp-token-collection-response-schema.json
slug: hubspot-marketing-emal-smtp-token-collection-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A paginated collection of SMTP tokens\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The list of SMTP tokens\",\n      \"example\": [\n        {\n          \"id\": \"smtp-token-abc123\",\n          \"campaignName\": \"Password Reset Emails\",\n          \"emailCampaignId\": \"campaign-xyz789\",\n          \"createContact\": true,\n          \"createdAt\": \"2024-01-15T10:30:00.000Z\",\n          \"createdBy\": \"user@example.com\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Represents an SMTP API token for transactional email sending\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the SMTP token\",\n            \"example\": \"smtp-token-abc123\"\n          },\n          \"campaignName\": {\n            \"type\": \"string\",\n\
  \            \"description\": \"The name of the email campaign associated with this token\",\n            \"example\": \"Password Reset Emails\"\n          },\n          \"emailCampaignId\": {\n            \"type\": \"string\",\n            \"description\": \"The ID of the associated email campaign\",\n            \"example\": \"campaign-xyz789\"\n          },\n          \"createContact\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether sending an email creates a contact if one doesn't exist\",\n            \"example\": true\n          },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"description\": \"When the token was created\",\n            \"format\": \"date-time\",\n            \"example\": \"2024-01-15T10:30:00.000Z\"\n          },\n          \"createdBy\": {\n            \"type\": \"string\",\n            \"description\": \"The user or application that created the token\",\n            \"example\": \"user@example.com\"\
  \n          }\n        },\n        \"required\": [\n          \"id\",\n          \"createdAt\",\n          \"createdBy\",\n          \"campaignName\",\n          \"createContact\"\n        ]\n      }\n    },\n    \"paging\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination information\",\n      \"properties\": {\n        \"next\": {\n          \"type\": \"object\",\n          \"description\": \"Information about the next page\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\": \"Cursor for the next page\",\n              \"example\": \"c210cC10b2tlbi1hYmMxMjM%3D\"\n            },\n            \"link\": {\n              \"type\": \"string\",\n              \"description\": \"Link to the next page\",\n              \"example\": \"https://app.hubspot.com/contacts/12345\"\n            }\n          },\n          \"required\": [\n            \"after\"\n          ]\n        }\n      }\n    }\n  },\n\
  \  \"required\": [\n    \"results\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SmtpTokenCollectionResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-marketing-emal-smtp-token-collection-response-schema.json
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
title: SmtpTokenCollectionResponse
---
