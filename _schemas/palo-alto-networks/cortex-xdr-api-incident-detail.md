---
description: IncidentDetail schema from Palo Alto Networks Cortex XDR REST API
layout: schema
name: IncidentDetail
properties_list: []
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/cortex-xdr-api-incident-detail-schema.json
slug: cortex-xdr-api-incident-detail
source_filename: cortex-xdr-api-incident-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentDetail\",\n  \"description\": \"IncidentDetail schema from Palo Alto Networks Cortex XDR REST API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-incident-detail-schema.json\",\n  \"allOf\": [\n    {\n      \"type\": \"object\",\n      \"description\": \"A Cortex XDR incident grouping related alerts.\",\n      \"properties\": {\n        \"incident_id\": {\n          \"type\": \"string\"\n        },\n        \"incident_name\": {\n          \"type\": \"string\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"new\",\n            \"under_investigation\",\n            \"resolved_threat_handled\",\n            \"resolved_known_issue\",\n            \"resolved_duplicate\",\n         \
  \   \"resolved_false_positive\",\n            \"resolved_other\"\n          ]\n        },\n        \"severity\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"critical\",\n            \"high\",\n            \"medium\",\n            \"low\",\n            \"informational\",\n            \"unknown\"\n          ]\n        },\n        \"assigned_user_mail\": {\n          \"type\": \"string\"\n        },\n        \"assigned_user_pretty_name\": {\n          \"type\": \"string\"\n        },\n        \"alert_count\": {\n          \"type\": \"integer\"\n        },\n        \"low_severity_alert_count\": {\n          \"type\": \"integer\"\n        },\n        \"med_severity_alert_count\": {\n          \"type\": \"integer\"\n        },\n        \"high_severity_alert_count\": {\n          \"type\": \"integer\"\n        },\n        \"critical_severity_alert_count\": {\n          \"type\": \"integer\"\n        },\n        \"user_count\": {\n          \"type\": \"integer\"\n\
  \        },\n        \"host_count\": {\n          \"type\": \"integer\"\n        },\n        \"creation_time\": {\n          \"type\": \"integer\",\n          \"description\": \"Incident creation timestamp as Unix epoch milliseconds.\"\n        },\n        \"modification_time\": {\n          \"type\": \"integer\",\n          \"description\": \"Last modification timestamp as Unix epoch milliseconds.\"\n        },\n        \"detection_time\": {\n          \"type\": \"integer\"\n        },\n        \"starred\": {\n          \"type\": \"boolean\"\n        },\n        \"xdr_url\": {\n          \"type\": \"string\",\n          \"description\": \"Direct URL to the incident in the XDR console.\"\n        },\n        \"rule_based_score\": {\n          \"type\": \"integer\"\n        },\n        \"manual_score\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    {\n      \"type\": \"object\",\n      \"properties\": {\n        \"network_artifacts\": {\n          \"type\": \"object\"\
  \n        },\n        \"file_artifacts\": {\n          \"type\": \"object\"\n        },\n        \"hosts\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"users\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"incident_sources\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"mitre_tactics_ids_and_names\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"mitre_techniques_ids_and_names\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/cortex-xdr-api-incident-detail-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IncidentDetail
---
