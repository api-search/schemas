---
description: Represents an incident in Enterprise Manager. Incidents are actionable issues detected by monitoring rules, correlated from one or more events.
layout: schema
name: Incident
properties_list:
- description: Unique identifier of the incident.
  name: incidentId
  type: string
- description: Brief summary of the incident.
  name: summary
  type: string
- description: Severity level of the incident.
  name: severity
  type: string
- description: Priority assigned to the incident.
  name: priority
  type: string
- description: Current status of the incident.
  name: status
  type: string
- description: Category of the incident.
  name: category
  type: string
- description: Name of the target associated with this incident.
  name: targetName
  type: string
- description: Type of the target associated with this incident.
  name: targetType
  type: string
- description: Current escalation level of the incident.
  name: escalationLevel
  type: integer
- description: Username of the incident owner or assignee.
  name: owner
  type: string
- description: Username of the person who acknowledged the incident.
  name: acknowledgedBy
  type: string
- description: Resolution state providing closure details.
  name: resolutionState
  type: string
- description: Name of the incident rule set that created this incident.
  name: ruleSetName
  type: string
- description: Timestamp when the incident was first raised.
  name: timeRaised
  type: string
- description: Timestamp of the last incident update.
  name: timeUpdated
  type: string
- description: Timestamp when the incident was resolved.
  name: timeResolved
  type: string
- description: Number of events correlated into this incident.
  name: eventCount
  type: integer
- description: Canonical URI for this incident resource.
  name: canonicalLink
  type: string
provider_name: Oracle Enterprise Manager
provider_slug: oracle-enterprise-manager
schema_file: json-schema/oracle-enterprise-manager-cloud-control-incident-schema.json
slug: oracle-enterprise-manager-cloud-control-incident
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Incident\",\n  \"type\": \"object\",\n  \"description\": \"Represents an incident in Enterprise Manager. Incidents are actionable issues detected by monitoring rules, correlated from one or more events.\",\n  \"properties\": {\n    \"incidentId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the incident.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Brief summary of the incident.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level of the incident.\"\n    },\n    \"priority\": {\n      \"type\": \"string\",\n      \"description\": \"Priority assigned to the incident.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the incident.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Category\
  \ of the incident.\"\n    },\n    \"targetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the target associated with this incident.\"\n    },\n    \"targetType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the target associated with this incident.\"\n    },\n    \"escalationLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Current escalation level of the incident.\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the incident owner or assignee.\"\n    },\n    \"acknowledgedBy\": {\n      \"type\": \"string\",\n      \"description\": \"Username of the person who acknowledged the incident.\"\n    },\n    \"resolutionState\": {\n      \"type\": \"string\",\n      \"description\": \"Resolution state providing closure details.\"\n    },\n    \"ruleSetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the incident rule set that created this incident.\"\n    },\n\
  \    \"timeRaised\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the incident was first raised.\"\n    },\n    \"timeUpdated\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp of the last incident update.\"\n    },\n    \"timeResolved\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the incident was resolved.\"\n    },\n    \"eventCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of events correlated into this incident.\"\n    },\n    \"canonicalLink\": {\n      \"type\": \"string\",\n      \"description\": \"Canonical URI for this incident resource.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-enterprise-manager/refs/heads/main/json-schema/oracle-enterprise-manager-cloud-control-incident-schema.json
tags:
- Cloud Management
- Database Management
- Enterprise Management
- Infrastructure Management
- Monitoring
- Oracle
title: Incident
---
