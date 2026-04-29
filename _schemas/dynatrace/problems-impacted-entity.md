---
description: A monitored entity that is impacted by the problem.
layout: schema
name: ImpactedEntity
properties_list:
- description: The Dynatrace entity ID of the impacted entity, in the format TYPE-HEXADECIMALID, e.g., SERVICE-1234567890ABCDEF.
  name: Entity
  type: string
- description: The display name of the impacted entity.
  name: Name
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-impacted-entity-schema.json
slug: problems-impacted-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-impacted-entity-schema.json\",\n  \"title\": \"ImpactedEntity\",\n  \"description\": \"A monitored entity that is impacted by the problem.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entity\": {\n      \"type\": \"string\",\n      \"description\": \"The Dynatrace entity ID of the impacted entity, in the format TYPE-HEXADECIMALID, e.g., SERVICE-1234567890ABCDEF.\",\n      \"example\": \"SERVICE-ABCDEF1234567890\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the impacted entity.\",\n      \"example\": \"payment-service\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-impacted-entity-schema.json
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
title: ImpactedEntity
---
