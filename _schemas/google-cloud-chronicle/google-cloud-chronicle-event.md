---
description: Schema for a Chronicle Unified Data Model (UDM) event, representing a normalized security telemetry event.
layout: schema
name: Google Cloud Chronicle UDM Event
properties_list:
- description: Event metadata including type, timestamps, and identifiers
  name: metadata
  type: object
- description: The entity that initiated the event
  name: principal
  type: object
- description: The entity that the event targets
  name: target
  type: object
- description: The source entity in network events
  name: src
  type: object
- description: The entity that observed or reported the event
  name: observer
  type: object
- description: Security results associated with the event
  name: securityResult
  type: array
- description: Network-related event information
  name: network
  type: object
provider_name: Google Cloud Chronicle
provider_slug: google-cloud-chronicle
schema_file: json-schema/google-cloud-chronicle-event-schema.json
slug: google-cloud-chronicle-event
source_filename: google-cloud-chronicle-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://cloud.google.com/schemas/chronicle/event.json\",\n  \"title\": \"Google Cloud Chronicle UDM Event\",\n  \"description\": \"Schema for a Chronicle Unified Data Model (UDM) event, representing a normalized security telemetry event.\",\n  \"type\": \"object\",\n  \"required\": [\"metadata\"],\n  \"properties\": {\n    \"metadata\": {\n      \"$ref\": \"#/$defs/Metadata\",\n      \"description\": \"Event metadata including type, timestamps, and identifiers\"\n    },\n    \"principal\": {\n      \"$ref\": \"#/$defs/Entity\",\n      \"description\": \"The entity that initiated the event\"\n    },\n    \"target\": {\n      \"$ref\": \"#/$defs/Entity\",\n      \"description\": \"The entity that the event targets\"\n    },\n    \"src\": {\n      \"$ref\": \"#/$defs/Entity\",\n      \"description\": \"The source entity in network events\"\n    },\n    \"observer\": {\n      \"$ref\": \"#/$defs/Entity\"\
  ,\n      \"description\": \"The entity that observed or reported the event\"\n    },\n    \"securityResult\": {\n      \"type\": \"array\",\n      \"description\": \"Security results associated with the event\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SecurityResult\"\n      }\n    },\n    \"network\": {\n      \"$ref\": \"#/$defs/Network\",\n      \"description\": \"Network-related event information\"\n    }\n  },\n  \"$defs\": {\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Event metadata\",\n      \"required\": [\"eventType\"],\n      \"properties\": {\n        \"eventType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of the event\",\n          \"enum\": [\n            \"NETWORK_CONNECTION\",\n            \"NETWORK_HTTP\",\n            \"NETWORK_DNS\",\n            \"FILE_CREATION\",\n            \"FILE_DELETION\",\n            \"FILE_MODIFICATION\",\n            \"PROCESS_LAUNCH\",\n            \"PROCESS_TERMINATION\"\
  ,\n            \"USER_LOGIN\",\n            \"USER_LOGOUT\",\n            \"REGISTRY_CREATION\",\n            \"REGISTRY_MODIFICATION\",\n            \"GENERIC_EVENT\",\n            \"STATUS_UPDATE\"\n          ]\n        },\n        \"eventTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp of the event\"\n        },\n        \"collectedTimestamp\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"The timestamp when the event was collected\"\n        },\n        \"productName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the product that generated the event\"\n        },\n        \"vendorName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the vendor of the product\"\n        },\n        \"productLogId\": {\n          \"type\": \"string\",\n          \"description\": \"Product-specific log\
  \ identifier\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the event\"\n        }\n      }\n    },\n    \"Entity\": {\n      \"type\": \"object\",\n      \"description\": \"An entity (host, user, process, etc.)\",\n      \"properties\": {\n        \"hostname\": {\n          \"type\": \"string\",\n          \"description\": \"The hostname of the entity\"\n        },\n        \"ip\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"IP addresses associated with the entity\"\n        },\n        \"mac\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"MAC addresses associated with the entity\"\n        },\n        \"user\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"userid\": {\n              \"type\": \"string\"\
  \n            },\n            \"emailAddresses\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            }\n          }\n        },\n        \"process\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"pid\": {\n              \"type\": \"string\"\n            },\n            \"file\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"fullPath\": {\n                  \"type\": \"string\"\n                },\n                \"sha256\": {\n                  \"type\": \"string\"\n                }\n              }\n            },\n            \"commandLine\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"port\": {\n          \"type\": \"integer\",\n          \"description\": \"The port number\"\n        }\n      }\n    },\n    \"SecurityResult\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A security result associated with the event\",\n      \"properties\": {\n        \"action\": {\n          \"type\": \"string\",\n          \"enum\": [\"ALLOW\", \"BLOCK\", \"QUARANTINE\", \"UNKNOWN_ACTION\"]\n        },\n        \"severity\": {\n          \"type\": \"string\",\n          \"enum\": [\"INFORMATIONAL\", \"LOW\", \"MEDIUM\", \"HIGH\", \"CRITICAL\"]\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"The category of the security result\"\n        },\n        \"summary\": {\n          \"type\": \"string\",\n          \"description\": \"Summary of the security result\"\n        },\n        \"ruleName\": {\n          \"type\": \"string\",\n          \"description\": \"The rule that triggered the security result\"\n        }\n      }\n    },\n    \"Network\": {\n      \"type\": \"object\",\n      \"description\": \"Network event information\",\n      \"properties\": {\n        \"ipProtocol\": {\n          \"type\": \"string\"\
  ,\n          \"enum\": [\"TCP\", \"UDP\", \"ICMP\"]\n        },\n        \"applicationProtocol\": {\n          \"type\": \"string\",\n          \"enum\": [\"HTTP\", \"HTTPS\", \"DNS\", \"SMTP\", \"SSH\", \"FTP\"]\n        },\n        \"sentBytes\": {\n          \"type\": \"integer\"\n        },\n        \"receivedBytes\": {\n          \"type\": \"integer\"\n        },\n        \"direction\": {\n          \"type\": \"string\",\n          \"enum\": [\"INBOUND\", \"OUTBOUND\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-chronicle/refs/heads/main/json-schema/google-cloud-chronicle-event-schema.json
tags:
- Incident Response
- Log Management
- Security Analytics
- Security Operations
- SIEM
- Threat Detection
title: Google Cloud Chronicle UDM Event
---
