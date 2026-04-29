---
description: The payload structure for pre-normalized event data ingestion directly into the XSIAM data lake. Contains all required routing metadata plus the normalized event content for direct dataset indexing.
layout: schema
name: EventDataPayload
properties_list:
- description: The target XSIAM dataset name for direct indexing. Must match an existing dataset schema in the XSIAM data lake.
  name: dataset
  type: string
- description: The vendor that produced the source event data.
  name: vendor
  type: string
- description: The product that generated the source event.
  name: product
  type: string
- description: The log type or event category identifier for schema selection during indexing.
  name: log_type
  type: string
- description: The original raw event content from the source system, preserved alongside normalized fields for audit and reprocessing purposes.
  name: raw_log
  type: string
- description: The ISO 8601 date-time string indicating when the original event occurred at the source system.
  name: timestamp
  type: string
- description: The XSIAM tenant identifier for multi-tenant data routing.
  name: tenant_id
  type: string
- description: A unique identifier for this event record used for deduplication and correlation reference.
  name: event_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsiam-data-ingestion-event-data-payload-schema.json
slug: cortex-xsiam-data-ingestion-event-data-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EventDataPayload\",\n  \"description\": \"The payload structure for pre-normalized event data ingestion directly into the XSIAM data lake. Contains all required routing metadata plus the normalized event content for direct dataset indexing.\\n\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-data-ingestion-event-data-payload-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"The target XSIAM dataset name for direct indexing. Must match an existing dataset schema in the XSIAM data lake.\\n\",\n      \"example\": \"authentication_events\"\n    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"The vendor that produced the source event data.\\n\",\n      \"example\": \"Microsoft\"\n    },\n    \"product\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"The product that generated the source event.\\n\",\n      \"example\": \"Active Directory\"\n    },\n    \"log_type\": {\n      \"type\": \"string\",\n      \"description\": \"The log type or event category identifier for schema selection during indexing.\\n\",\n      \"example\": \"authentication\"\n    },\n    \"raw_log\": {\n      \"type\": \"string\",\n      \"description\": \"The original raw event content from the source system, preserved alongside normalized fields for audit and reprocessing purposes.\\n\",\n      \"example\": \"{\\\"EventID\\\":4625,\\\"AccountName\\\":\\\"jsmith\\\",...}\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 date-time string indicating when the original event occurred at the source system.\\n\",\n      \"example\": \"2024-01-15T10:28:00.000Z\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The XSIAM tenant identifier for multi-tenant data routing.\\n\",\n      \"example\": \"xsiam-tenant-001\"\n    },\n    \"event_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this event record used for deduplication and correlation reference.\\n\",\n      \"example\": \"evt-20240115-102800-002\"\n    }\n  },\n  \"required\": [\n    \"dataset\",\n    \"vendor\",\n    \"product\",\n    \"log_type\",\n    \"raw_log\",\n    \"timestamp\",\n    \"tenant_id\",\n    \"event_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-data-ingestion-event-data-payload-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EventDataPayload
---
