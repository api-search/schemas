---
description: SOAP response containing session and security tokens.
layout: schema
name: SessionLogonResponse
properties_list:
- description: Session token to be passed as __sessiontoken cookie on subsequent requests.
  name: sessionToken
  type: string
- description: Security token to be passed as X-Security-Token header on subsequent requests.
  name: securityToken
  type: string
- description: Information about the authenticated session.
  name: sessionInfo
  type: object
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-classic-session-logon-response-schema.json
slug: adobe-campaign-classic-session-logon-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-session-logon-response-schema.json\",\n  \"title\": \"SessionLogonResponse\",\n  \"description\": \"SOAP response containing session and security tokens.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sessionToken\": {\n      \"type\": \"string\",\n      \"description\": \"Session token to be passed as __sessiontoken cookie on subsequent requests.\",\n      \"example\": \"example_value\"\n    },\n    \"securityToken\": {\n      \"type\": \"string\",\n      \"description\": \"Security token to be passed as X-Security-Token header on subsequent requests.\",\n      \"example\": \"example_value\"\n    },\n    \"sessionInfo\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the authenticated session.\",\n      \"properties\": {\n        \"serverInfo\"\
  : {\n          \"type\": \"string\"\n        },\n        \"timezone\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-classic-session-logon-response-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: SessionLogonResponse
---
