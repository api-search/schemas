---
description: A reference to an alerting profile (problem filter).
layout: schema
name: AlertingProfileStub
properties_list:
- description: The unique identifier of the alerting profile.
  name: id
  type: string
- description: The display name of the alerting profile.
  name: name
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-problems-v2-alerting-profile-stub-schema.json
slug: dynatrace-problems-v2-alerting-profile-stub
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A reference to an alerting profile (problem filter).\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the alerting profile.\",\n      \"example\": \"abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the alerting profile.\",\n      \"example\": \"Production Service\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlertingProfileStub\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-problems-v2-alerting-profile-stub-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: AlertingProfileStub
---
