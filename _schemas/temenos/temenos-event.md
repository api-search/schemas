---
description: Schema for Temenos banking events published through the event-driven architecture via Apache Kafka and JMS messaging. Covers business events, system events, and data replication events.
layout: schema
name: Temenos Banking Event
properties_list:
- description: Unique event identifier for deduplication and tracking
  name: eventId
  type: string
- description: Classification of the event type
  name: eventType
  type: string
- description: Source application or service that generated the event
  name: source
  type: string
- description: Correlation identifier for tracing related events across services
  name: correlationId
  type: string
- description: ISO 8601 timestamp when the event occurred
  name: timestamp
  type: string
- description: Event schema version for compatibility
  name: version
  type: string
- description: Event-specific payload data in JSON format
  name: payload
  type: object
- description: ''
  name: metadata
  type: object
provider_name: Temenos
provider_slug: temenos
schema_file: json-schema/temenos-event-schema.json
slug: temenos-event
source_filename: temenos-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://temenos.com/schemas/temenos/event.json\",\n  \"title\": \"Temenos Banking Event\",\n  \"description\": \"Schema for Temenos banking events published through the event-driven architecture via Apache Kafka and JMS messaging. Covers business events, system events, and data replication events.\",\n  \"type\": \"object\",\n  \"required\": [\"eventId\", \"eventType\", \"timestamp\"],\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique event identifier for deduplication and tracking\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the event type\",\n      \"enum\": [\n        \"account.created\",\n        \"account.closed\",\n        \"account.status.changed\",\n        \"payment.order.accepted\",\n        \"payment.order.confirmed\",\n        \"payment.order.failed\",\n        \"customer.onboarded\"\
  ,\n        \"customer.updated\",\n        \"customer.kyc.changed\",\n        \"transaction.committed\",\n        \"compliance.sanction.alert\",\n        \"compliance.risk.changed\",\n        \"data.replication\",\n        \"system.health\",\n        \"system.config.changed\"\n      ]\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source application or service that generated the event\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Correlation identifier for tracing related events across services\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the event occurred\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Event schema version for compatibility\",\n      \"pattern\": \"^[0-9]+\\\\.[0-9]+$\"\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"Event-specific\
  \ payload data in JSON format\",\n      \"additionalProperties\": true\n    },\n    \"metadata\": {\n      \"$ref\": \"#/$defs/EventMetadata\"\n    }\n  },\n  \"$defs\": {\n    \"EventMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"Additional metadata about the event for processing and routing\",\n      \"properties\": {\n        \"tenantId\": {\n          \"type\": \"string\",\n          \"description\": \"Multi-tenant identifier\"\n        },\n        \"userId\": {\n          \"type\": \"string\",\n          \"description\": \"User who triggered the event\"\n        },\n        \"channel\": {\n          \"type\": \"string\",\n          \"description\": \"Channel through which the event originated\",\n          \"enum\": [\"API\", \"ONLINE_BANKING\", \"MOBILE\", \"BRANCH\", \"ATM\", \"BATCH\", \"SYSTEM\"]\n        },\n        \"priority\": {\n          \"type\": \"string\",\n          \"description\": \"Event processing priority\",\n          \"enum\": [\"LOW\", \"\
  NORMAL\", \"HIGH\", \"CRITICAL\"]\n        },\n        \"retryCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of delivery retry attempts\",\n          \"minimum\": 0\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temenos/refs/heads/main/json-schema/temenos-event-schema.json
tags:
- Banking
- Cloud Banking
- Core Banking
- Digital Banking
- Financial Services
- Fintech
- Open Banking
- Payments
- Wealth Management
title: Temenos Banking Event
---
