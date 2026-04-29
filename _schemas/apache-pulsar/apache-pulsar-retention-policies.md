---
description: RetentionPolicies schema from Apache Pulsar
layout: schema
name: RetentionPolicies
properties_list:
- description: ''
  name: retentionTimeInMinutes
  type: integer
- description: ''
  name: retentionSizeInMB
  type: integer
provider_name: Apache Pulsar
provider_slug: apache-pulsar
schema_file: json-schema/apache-pulsar-retention-policies-schema.json
slug: apache-pulsar-retention-policies
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-retention-policies-schema.json\",\n  \"title\": \"RetentionPolicies\",\n  \"description\": \"RetentionPolicies schema from Apache Pulsar\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"retentionTimeInMinutes\": {\n      \"type\": \"integer\"\n    },\n    \"retentionSizeInMB\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-pulsar/refs/heads/main/json-schema/apache-pulsar-retention-policies-schema.json
tags:
- Cloud Native
- Messaging
- Multi-Tenant
- Pub-Sub
- Streaming
- Apache
- Open Source
title: RetentionPolicies
---
