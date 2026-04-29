---
description: IncidentSummary schema from Palo Alto Networks Enterprise DLP API
layout: schema
name: IncidentSummary
properties_list:
- description: Total number of incidents in the reporting period.
  name: total_incidents
  type: integer
- description: Number of incidents still in open status.
  name: open_incidents
  type: integer
- description: Number of resolved incidents.
  name: resolved_incidents
  type: integer
- description: Incident count breakdown by severity.
  name: by_severity
  type: object
- description: Incident count breakdown by detection channel.
  name: by_channel
  type: object
- description: Most frequently triggered data patterns.
  name: top_data_patterns
  type: array
- description: Users with the most incidents.
  name: top_users
  type: array
- description: Time range for the summary report.
  name: reporting_period
  type: object
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/dlp-api-incident-summary-schema.json
slug: dlp-api-incident-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IncidentSummary\",\n  \"description\": \"IncidentSummary schema from Palo Alto Networks Enterprise DLP API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-incident-summary-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_incidents\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of incidents in the reporting period.\"\n    },\n    \"open_incidents\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of incidents still in open status.\"\n    },\n    \"resolved_incidents\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of resolved incidents.\"\n    },\n    \"by_severity\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"critical\": {\n          \"type\": \"integer\"\n        },\n        \"high\": {\n          \"type\": \"\
  integer\"\n        },\n        \"medium\": {\n          \"type\": \"integer\"\n        },\n        \"low\": {\n          \"type\": \"integer\"\n        },\n        \"informational\": {\n          \"type\": \"integer\"\n        }\n      },\n      \"description\": \"Incident count breakdown by severity.\"\n    },\n    \"by_channel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"web\": {\n          \"type\": \"integer\"\n        },\n        \"ssl\": {\n          \"type\": \"integer\"\n        },\n        \"saas\": {\n          \"type\": \"integer\"\n        },\n        \"email\": {\n          \"type\": \"integer\"\n        },\n        \"endpoint\": {\n          \"type\": \"integer\"\n        }\n      },\n      \"description\": \"Incident count breakdown by detection channel.\"\n    },\n    \"top_data_patterns\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"pattern_name\": {\n            \"type\"\
  : \"string\"\n          },\n          \"incident_count\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"description\": \"Most frequently triggered data patterns.\"\n    },\n    \"top_users\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"user\": {\n            \"type\": \"string\"\n          },\n          \"incident_count\": {\n            \"type\": \"integer\"\n          }\n        }\n      },\n      \"description\": \"Users with the most incidents.\"\n    },\n    \"reporting_period\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"start_time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"end_time\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      },\n      \"description\": \"Time range for the summary report.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/dlp-api-incident-summary-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: IncidentSummary
---
