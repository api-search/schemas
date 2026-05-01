---
description: Schema for a Debezium change data capture event envelope, containing before/after state and source metadata.
layout: schema
name: Debezium Change Event
properties_list:
- description: The Kafka Connect schema for the change event
  name: schema
  type: object
- description: The change event payload
  name: payload
  type: object
provider_name: Debezium
provider_slug: debezium
schema_file: json-schema/debezium-change-event.json
slug: debezium-change-event
source_filename: debezium-change-event.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/schemas/debezium/debezium-change-event.json\",\n  \"title\": \"Debezium Change Event\",\n  \"description\": \"Schema for a Debezium change data capture event envelope, containing before/after state and source metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"schema\": {\n      \"type\": \"object\",\n      \"description\": \"The Kafka Connect schema for the change event\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\"\n        },\n        \"fields\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\"\n          }\n        },\n        \"optional\": {\n          \"type\": \"boolean\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"payload\": {\n      \"type\": \"object\",\n      \"description\": \"The change event payload\",\n    \
  \  \"properties\": {\n        \"before\": {\n          \"description\": \"Row state before the change (null for inserts)\",\n          \"oneOf\": [\n            { \"type\": \"object\" },\n            { \"type\": \"null\" }\n          ]\n        },\n        \"after\": {\n          \"description\": \"Row state after the change (null for deletes)\",\n          \"oneOf\": [\n            { \"type\": \"object\" },\n            { \"type\": \"null\" }\n          ]\n        },\n        \"source\": {\n          \"type\": \"object\",\n          \"description\": \"Source metadata about the change event\",\n          \"properties\": {\n            \"version\": {\n              \"type\": \"string\",\n              \"description\": \"Debezium version\"\n            },\n            \"connector\": {\n              \"type\": \"string\",\n              \"description\": \"Connector type (mysql, postgresql, mongodb, etc.)\"\n            },\n            \"name\": {\n              \"type\": \"string\",\n   \
  \           \"description\": \"Logical name of the database server\"\n            },\n            \"ts_ms\": {\n              \"type\": \"integer\",\n              \"description\": \"Timestamp of the change in the source database (milliseconds)\"\n            },\n            \"snapshot\": {\n              \"type\": \"string\",\n              \"description\": \"Whether this event is from a snapshot\"\n            },\n            \"db\": {\n              \"type\": \"string\",\n              \"description\": \"Database name\"\n            },\n            \"schema\": {\n              \"type\": \"string\",\n              \"description\": \"Schema name\"\n            },\n            \"table\": {\n              \"type\": \"string\",\n              \"description\": \"Table name\"\n            },\n            \"txId\": {\n              \"type\": \"integer\",\n              \"description\": \"Transaction ID\"\n            },\n            \"lsn\": {\n              \"type\": \"integer\",\n       \
  \       \"description\": \"Log sequence number (PostgreSQL)\"\n            },\n            \"file\": {\n              \"type\": \"string\",\n              \"description\": \"Binlog filename (MySQL)\"\n            },\n            \"pos\": {\n              \"type\": \"integer\",\n              \"description\": \"Binlog position (MySQL)\"\n            },\n            \"row\": {\n              \"type\": \"integer\",\n              \"description\": \"Row within the event\"\n            }\n          }\n        },\n        \"op\": {\n          \"type\": \"string\",\n          \"enum\": [\"c\", \"u\", \"d\", \"r\", \"t\"],\n          \"description\": \"Operation type: c=create, u=update, d=delete, r=read (snapshot), t=truncate\"\n        },\n        \"ts_ms\": {\n          \"type\": \"integer\",\n          \"description\": \"Timestamp when Debezium processed the event (milliseconds)\"\n        },\n        \"transaction\": {\n          \"type\": \"object\",\n          \"description\": \"Transaction\
  \ metadata\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"string\"\n            },\n            \"total_order\": {\n              \"type\": \"integer\"\n            },\n            \"data_collection_order\": {\n              \"type\": \"integer\"\n            }\n          }\n        }\n      },\n      \"required\": [\"op\", \"source\"]\n    }\n  },\n  \"required\": [\"payload\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/debezium/refs/heads/main/json-schema/debezium-change-event.json
tags:
- Apache Kafka
- CDC
- Change Data Capture
- Databases
- Event Streaming
- Open Source
title: Debezium Change Event
---
