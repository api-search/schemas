---
description: 'Array of field paths specifying which fields to update. Uses dot notation for nested fields (e.g., "config.revision", "metadata.tags"). **Field Path Rules:** - Use dot notation for nested objects: `parent.child.field` - Escape special characters: `field\.with\.dots`, `field\:with\:colons` - Array elements not directly addressable - Object names can be specified directly (e.g., "config.content.read.objects.contacts") - The * operator in paths like "config.content.read.objects.*" allows you to specify any object name - Example: "config.content.read.objects.*" pattern allows "config.content.read.objects.contacts", "config.content.read.objects.leads", etc.'
layout: schema
name: UpdateMask
properties_list: []
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-update-mask-schema.json
slug: ampersand-api-update-mask
source_filename: ampersand-api-update-mask-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-update-mask-schema.json\",\n  \"title\": \"UpdateMask\",\n  \"description\": \"Array of field paths specifying which fields to update.\\nUses dot notation for nested fields (e.g., \\\"config.revision\\\", \\\"metadata.tags\\\").\\n\\n**Field Path Rules:**\\n- Use dot notation for nested objects: `parent.child.field`\\n- Escape special characters: `field\\\\.with\\\\.dots`, `field\\\\:with\\\\:colons`\\n- Array elements not directly addressable\\n- Object names can be specified directly (e.g., \\\"config.content.read.objects.contacts\\\")\\n- The * operator in paths like \\\"config.content.read.objects.*\\\" allows you to specify any object name\\n  - Example: \\\"config.content.read.objects.*\\\" pattern allows \\\"config.content.read.objects.contacts\\\", \\\"config.content.read.objects.leads\\\
  \", etc.\\n\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\"\n  },\n  \"example\": [\n    \"name\",\n    \"config.content.read.objects.contacts\",\n    \"config.content.write.objects.leads\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-update-mask-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: UpdateMask
---
