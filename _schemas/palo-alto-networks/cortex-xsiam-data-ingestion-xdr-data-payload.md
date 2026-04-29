---
description: The payload structure for XDR data forwarding from integrated Palo Alto Networks products. Contains product identification, tenant context, event identification, and the forwarded telemetry content for correlation in the XSIAM unified data lake.
layout: schema
name: XdrDataPayload
properties_list:
- description: The target XSIAM dataset name for the forwarded XDR data.
  name: dataset
  type: string
- description: The Palo Alto Networks product vendor designation for the forwarding source. Typically 'Palo Alto Networks'.
  name: vendor
  type: string
- description: The specific Palo Alto Networks product forwarding XDR data, such as Cortex XDR Agent, PAN-OS, Prisma Access, or Strata Logging Service.
  name: product
  type: string
- description: The XDR data type or telemetry category being forwarded (e.g., xdr_data, endpoint_event, network_event).
  name: log_type
  type: string
- description: The raw XDR telemetry content as serialized JSON from the forwarding product. Contains all available event fields from the source product's data model.
  name: raw_log
  type: string
- description: The ISO 8601 date-time string indicating when the XDR event was captured by the source product.
  name: timestamp
  type: string
- description: The XSIAM tenant identifier to which this XDR data belongs. Ensures forwarded data is routed to the correct tenant environment in multi-tenant deployments.
  name: tenant_id
  type: string
- description: A unique identifier for this forwarded XDR event, used for deduplication, correlation, and audit trail tracking.
  name: event_id
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xsiam-data-ingestion-xdr-data-payload-schema.json
slug: cortex-xsiam-data-ingestion-xdr-data-payload
source_filename: cortex-xsiam-data-ingestion-xdr-data-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"XdrDataPayload\",\n  \"description\": \"The payload structure for XDR data forwarding from integrated Palo Alto Networks products. Contains product identification, tenant context, event identification, and the forwarded telemetry content for correlation in the XSIAM unified data lake.\\n\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-data-ingestion-xdr-data-payload-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dataset\": {\n      \"type\": \"string\",\n      \"description\": \"The target XSIAM dataset name for the forwarded XDR data.\\n\",\n      \"example\": \"xdr_agent_raw\"\n    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"The Palo Alto Networks product vendor designation for the forwarding source. Typically 'Palo Alto Networks'.\\n\",\n      \"example\": \"\
  Palo Alto Networks\"\n    },\n    \"product\": {\n      \"type\": \"string\",\n      \"description\": \"The specific Palo Alto Networks product forwarding XDR data, such as Cortex XDR Agent, PAN-OS, Prisma Access, or Strata Logging Service.\\n\",\n      \"example\": \"Cortex XDR Agent\"\n    },\n    \"log_type\": {\n      \"type\": \"string\",\n      \"description\": \"The XDR data type or telemetry category being forwarded (e.g., xdr_data, endpoint_event, network_event).\\n\",\n      \"example\": \"xdr_data\"\n    },\n    \"raw_log\": {\n      \"type\": \"string\",\n      \"description\": \"The raw XDR telemetry content as serialized JSON from the forwarding product. Contains all available event fields from the source product's data model.\\n\",\n      \"example\": \"{\\\"type\\\":\\\"PROCESS_EVENT\\\",\\\"hostname\\\":\\\"WORKSTATION-042\\\",...}\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 date-time\
  \ string indicating when the XDR event was captured by the source product.\\n\",\n      \"example\": \"2024-01-15T10:35:00.000Z\"\n    },\n    \"tenant_id\": {\n      \"type\": \"string\",\n      \"description\": \"The XSIAM tenant identifier to which this XDR data belongs. Ensures forwarded data is routed to the correct tenant environment in multi-tenant deployments.\\n\",\n      \"example\": \"xsiam-tenant-001\"\n    },\n    \"event_id\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this forwarded XDR event, used for deduplication, correlation, and audit trail tracking.\\n\",\n      \"example\": \"evt-20240115-103500-003\"\n    }\n  },\n  \"required\": [\n    \"dataset\",\n    \"vendor\",\n    \"product\",\n    \"log_type\",\n    \"raw_log\",\n    \"timestamp\",\n    \"tenant_id\",\n    \"event_id\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xsiam-data-ingestion-xdr-data-payload-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: XdrDataPayload
---
