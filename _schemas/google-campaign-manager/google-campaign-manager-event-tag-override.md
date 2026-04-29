---
description: Event tag override configuration.
layout: schema
name: EventTagOverride
properties_list:
- description: ID of the event tag that is overridden.
  name: id
  type: string
- description: Whether this override is enabled.
  name: enabled
  type: boolean
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-event-tag-override-schema.json
slug: google-campaign-manager-event-tag-override
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventTagOverride\",\n  \"type\": \"object\",\n  \"description\": \"Event tag override configuration.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the event tag that is overridden.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this override is enabled.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-event-tag-override-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: EventTagOverride
---
