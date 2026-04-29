---
description: A comment or note attached to an incident, providing investigation details or remediation notes.
layout: schema
name: Annotation
properties_list:
- description: Unique identifier of the annotation.
  name: annotationId
  type: string
- description: Summary text of the annotation.
  name: summary
  type: string
- description: Detailed content of the annotation.
  name: details
  type: string
- description: Username of the annotation author.
  name: author
  type: string
- description: Timestamp when the annotation was created.
  name: timeCreated
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-annotation-schema.json
slug: oracle-enterprise-manager-cloud-control-annotation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Annotation\",\n  \"type\": \"object\",\n  \"description\": \"A comment or note attached to an incident, providing investigation details or remediation notes.\",\n  \"properties\": {\n    \"annotationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the annotation.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Summary text of the annotation.\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed content of the annotation.\"\n    },\n    \"author\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the annotation author.\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the annotation was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-annotation-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: Annotation
---
