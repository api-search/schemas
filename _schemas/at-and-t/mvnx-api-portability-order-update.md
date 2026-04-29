---
description: PortabilityOrderUpdate schema from AT&T API
layout: schema
name: PortabilityOrderUpdate
properties_list:
- description: Updated requested completion date
  name: requestedCompletionDate
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-portability-order-update-schema.json
slug: mvnx-api-portability-order-update
source_filename: mvnx-api-portability-order-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-update-schema.json\",\n  \"title\": \"PortabilityOrderUpdate\",\n  \"description\": \"PortabilityOrderUpdate schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestedCompletionDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Updated requested completion date\",\n      \"example\": \"2026-04-25T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/mvnx-api-portability-order-update-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: PortabilityOrderUpdate
---
