---
description: SalesNavigatorProfileAssociationKey from LinkedIn API
layout: schema
name: SalesNavigatorProfileAssociationKey
properties_list:
- description: ID of the CRM partner that synced with Sales Navigator
  name: partner
  type: string
- description: ID of the CRM instance that synced with Sales Navigator
  name: instanceId
  type: string
- description: ID of the CRM record
  name: recordId
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-sales-navigator-sales-navigator-profile-association-key-schema.json
slug: linkedin-sales-navigator-sales-navigator-profile-association-key
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-navigator-profile-association-key-schema.json\",\n  \"title\": \"SalesNavigatorProfileAssociationKey\",\n  \"description\": \"SalesNavigatorProfileAssociationKey from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"partner\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the CRM partner that synced with Sales Navigator\",\n      \"example\": \"salesforce\"\n    },\n    \"instanceId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the CRM instance that synced with Sales Navigator\",\n      \"example\": \"sf-instance-001\"\n    },\n    \"recordId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the CRM record\",\n      \"example\": \"contact-12345\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-sales-navigator-sales-navigator-profile-association-key-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: SalesNavigatorProfileAssociationKey
---
