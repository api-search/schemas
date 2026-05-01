---
description: An email address with optional display name used in Global Relay email archiving.
layout: schema
name: Global Relay Email Address
properties_list:
- description: Email address
  name: address
  type: string
- description: Display name associated with the email address
  name: displayName
  type: string
provider_name: Global Relay
provider_slug: global-relay
schema_file: json-schema/global-relay-email-address.json
slug: global-relay-email-address
source_filename: global-relay-email-address.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"global-relay-email-address.json\",\n  \"title\": \"Global Relay Email Address\",\n  \"description\": \"An email address with optional display name used in Global Relay email archiving.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"address\"\n  ],\n  \"properties\": {\n    \"address\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name associated with the email address\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/global-relay/refs/heads/main/json-schema/global-relay-email-address.json
tags:
- Archiving
- Compliance
- Data Retention
- Email Security
- Regulatory Compliance
title: Global Relay Email Address
---
