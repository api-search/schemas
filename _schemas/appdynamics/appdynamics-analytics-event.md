---
description: Schema representing a custom analytics event and its schema definition for the AppDynamics Events Service.
layout: schema
name: AppDynamics Analytics Event
properties_list:
- description: The name of the custom event schema.
  name: schemaName
  type: string
- description: The schema definition for this event type.
  name: schema
  type: object
- description: Array of event data objects conforming to the schema.
  name: events
  type: array
provider_name: AppDynamics
provider_slug: appdynamics
schema_file: json-schema/appdynamics-analytics-event-schema.json
slug: appdynamics-analytics-event
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://appdynamics.com/schemas/appdynamics/analytics-event.json\",\n  \"title\": \"AppDynamics Analytics Event\",\n  \"description\": \"Schema representing a custom analytics event and its schema definition for the AppDynamics Events Service.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"EventSchemaField\": {\n      \"type\": \"object\",\n      \"description\": \"A field definition within a custom event schema.\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The data type of the field.\",\n          \"enum\": [\n            \"string\",\n            \"integer\",\n            \"float\",\n            \"boolean\",\n            \"date\"\n          ]\n        },\n        \"label\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable label for the field.\"\n        }\n\
  \      }\n    },\n    \"EventSchema\": {\n      \"type\": \"object\",\n      \"description\": \"A custom event schema definition for the Events Service.\",\n      \"required\": [\"schema\"],\n      \"properties\": {\n        \"schema\": {\n          \"type\": \"object\",\n          \"description\": \"The schema definition mapping field names to their type definitions.\",\n          \"additionalProperties\": {\n            \"$ref\": \"#/$defs/EventSchemaField\"\n          }\n        }\n      }\n    },\n    \"QueryResult\": {\n      \"type\": \"object\",\n      \"description\": \"The result of an ADQL query execution.\",\n      \"properties\": {\n        \"fields\": {\n          \"type\": \"array\",\n          \"description\": \"The column definitions for the query results.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"label\": {\n                \"type\": \"string\",\n                \"description\": \"The column label.\"\n\
  \              },\n              \"field\": {\n                \"type\": \"string\",\n                \"description\": \"The field name.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"The data type of the column.\"\n              }\n            }\n          }\n        },\n        \"results\": {\n          \"type\": \"array\",\n          \"description\": \"The data rows returned by the query.\",\n          \"items\": {\n            \"type\": \"array\"\n          }\n        },\n        \"moreData\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether additional data is available beyond the limit.\"\n        },\n        \"totalCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The total number of results matching the query.\",\n          \"minimum\": 0\n        }\n      }\n    }\n  },\n  \"properties\": {\n    \"schemaName\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The name of the custom event schema.\",\n      \"minLength\": 1,\n      \"maxLength\": 255,\n      \"pattern\": \"^[a-zA-Z][a-zA-Z0-9_]*$\"\n    },\n    \"schema\": {\n      \"$ref\": \"#/$defs/EventSchema\",\n      \"description\": \"The schema definition for this event type.\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"description\": \"Array of event data objects conforming to the schema.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/appdynamics/refs/heads/main/json-schema/appdynamics-analytics-event-schema.json
tags:
- APM
- Application Performance Monitoring
- Cisco
- Cloud Observability
- DevOps
- Monitoring
- Observability
- OpenTelemetry
title: AppDynamics Analytics Event
---
