---
description: An EPCIS 2.0 event capturing the state or movement of RFID-tagged objects in a supply chain
layout: schema
name: RFID EPC EPCIS Event
properties_list:
- description: EPCIS event type
  name: type
  type: string
- description: ISO 8601 timestamp when the event occurred
  name: eventTime
  type: string
- description: Time zone offset of the event (e.g., +00:00)
  name: eventTimeZoneOffset
  type: string
- description: List of EPCs involved in the event
  name: epcList
  type: array
- description: The action taken on the EPCs at this event
  name: action
  type: string
- description: Business step URI indicating the business process step (CBV vocabulary)
  name: bizStep
  type: string
- description: Disposition URI indicating the status of the objects (CBV vocabulary)
  name: disposition
  type: string
- description: ''
  name: readPoint
  type: object
- description: ''
  name: bizLocation
  type: object
- description: ''
  name: bizTransactionList
  type: array
- description: ''
  name: sensorElementList
  type: array
provider_name: RFID
provider_slug: rfid
schema_file: json-schema/rfid-epc-event-schema.json
slug: rfid-epc-event
source_filename: rfid-epc-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/rfid/main/json-schema/rfid-epc-event-schema.json\",\n  \"title\": \"RFID EPC EPCIS Event\",\n  \"description\": \"An EPCIS 2.0 event capturing the state or movement of RFID-tagged objects in a supply chain\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ObjectEvent\",\n        \"AggregationEvent\",\n        \"TransactionEvent\",\n        \"TransformationEvent\",\n        \"AssociationEvent\"\n      ],\n      \"description\": \"EPCIS event type\"\n    },\n    \"eventTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the event occurred\"\n    },\n    \"eventTimeZoneOffset\": {\n      \"type\": \"string\",\n      \"pattern\": \"^[+-]\\\\d{2}:\\\\d{2}$\",\n      \"description\": \"Time zone offset of the event\
  \ (e.g., +00:00)\"\n    },\n    \"epcList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"Electronic Product Code in URN format (e.g., urn:epc:id:sgtin:0614141.107346.2017)\"\n      },\n      \"description\": \"List of EPCs involved in the event\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\"ADD\", \"OBSERVE\", \"DELETE\"],\n      \"description\": \"The action taken on the EPCs at this event\"\n    },\n    \"bizStep\": {\n      \"type\": \"string\",\n      \"description\": \"Business step URI indicating the business process step (CBV vocabulary)\",\n      \"examples\": [\n        \"urn:epcglobal:cbv:bizstep:shipping\",\n        \"urn:epcglobal:cbv:bizstep:receiving\",\n        \"urn:epcglobal:cbv:bizstep:stocking\",\n        \"urn:epcglobal:cbv:bizstep:pos\"\n      ]\n    },\n    \"disposition\": {\n      \"type\": \"string\",\n      \"description\": \"Disposition URI indicating the status of\
  \ the objects (CBV vocabulary)\",\n      \"examples\": [\n        \"urn:epcglobal:cbv:disp:in_transit\",\n        \"urn:epcglobal:cbv:disp:in_progress\",\n        \"urn:epcglobal:cbv:disp:sellable_accessible\"\n      ]\n    },\n    \"readPoint\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"URI identifying the specific physical read point\"\n        }\n      },\n      \"required\": [\"id\"]\n    },\n    \"bizLocation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"URI identifying the business location (GLN or custom URI)\"\n        }\n      },\n      \"required\": [\"id\"]\n    },\n    \"bizTransactionList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": { \"type\": \"string\" },\n          \"bizTransaction\": { \"type\"\
  : \"string\" }\n        }\n      }\n    },\n    \"sensorElementList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Sensor data (temperature, humidity, etc.) associated with the event\"\n      }\n    }\n  },\n  \"required\": [\"type\", \"eventTime\", \"action\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rfid/refs/heads/main/json-schema/rfid-epc-event-schema.json
tags:
- RFID
- IoT
- Supply Chain
- Inventory Management
- Asset Tracking
- GS1
- EPCIS
title: RFID EPC EPCIS Event
---
