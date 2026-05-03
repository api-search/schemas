---
description: Schema for a SaaS Alerts security event detected across monitored SaaS applications
layout: schema
name: SaaS Alerts Security Event
properties_list:
- description: Unique event identifier
  name: eventId
  type: string
- description: Machine-readable event type classification
  name: eventType
  type: string
- description: Human-readable event description
  name: jointDesc
  type: string
- description: Event severity level
  name: alertStatus
  type: string
- description: SaaS application where the event occurred
  name: application
  type: string
- description: MSP customer/tenant identifier
  name: customerId
  type: string
- description: Customer organization name
  name: customerName
  type: string
- description: Affected user identifier (email address)
  name: userId
  type: string
- description: Source IP address of the event
  name: sourceIp
  type: string
- description: Event timestamp in ISO 8601 format
  name: timestamp
  type: string
- description: Additional event-specific details
  name: details
  type: object
provider_name: SaaS Alerts
provider_slug: saas-alerts
schema_file: json-schema/saas-alerts-security-event-schema.json
slug: saas-alerts-security-event
source_filename: saas-alerts-security-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/json-schema/saas-alerts-security-event-schema.json\",\n  \"title\": \"SaaS Alerts Security Event\",\n  \"description\": \"Schema for a SaaS Alerts security event detected across monitored SaaS applications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique event identifier\",\n      \"example\": \"evt_1234567890abcdef\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable event type classification\",\n      \"enum\": [\n        \"login.success\",\n        \"login.failure\",\n        \"cross.ip.connections\",\n        \"file.sharing.external\",\n        \"oauth.granted.permission\",\n        \"oauth.revoked.permission\",\n        \"admin.new.admin\",\n        \"admin.removed.admin\",\n      \
  \  \"mfa.disable\",\n        \"mfa.new.device\",\n        \"account.suspended\",\n        \"account.password.changed\",\n        \"policy.security.changed\",\n        \"mail.forwarding.added\",\n        \"mail.forwarding.removed\",\n        \"mail.rule.created\",\n        \"mail.rule.deleted\",\n        \"file.deleted\",\n        \"file.downloaded\",\n        \"file.uploaded\",\n        \"data.exfiltration\",\n        \"impossible.travel\",\n        \"brute.force.attack\",\n        \"api.access.granted\",\n        \"api.access.revoked\"\n      ],\n      \"example\": \"login.failure\"\n    },\n    \"jointDesc\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable event description\",\n      \"example\": \"IAM Event - Authentication Failure\"\n    },\n    \"alertStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Event severity level\",\n      \"enum\": [\"low\", \"medium\", \"critical\"],\n      \"example\": \"critical\"\n    },\n    \"application\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"SaaS application where the event occurred\",\n      \"enum\": [\n        \"microsoft365\",\n        \"google_workspace\",\n        \"salesforce\",\n        \"slack\",\n        \"dropbox\"\n      ],\n      \"example\": \"microsoft365\"\n    },\n    \"customerId\": {\n      \"type\": \"string\",\n      \"description\": \"MSP customer/tenant identifier\",\n      \"example\": \"cust_abc123\"\n    },\n    \"customerName\": {\n      \"type\": \"string\",\n      \"description\": \"Customer organization name\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Affected user identifier (email address)\",\n      \"example\": \"user@acme.com\"\n    },\n    \"sourceIp\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"Source IP address of the event\",\n      \"example\": \"198.51.100.42\"\n    },\n    \"timestamp\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Event timestamp in ISO 8601 format\",\n      \"example\": \"2024-01-15T14:23:11Z\"\n    },\n    \"details\": {\n      \"type\": \"object\",\n      \"description\": \"Additional event-specific details\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"eventId\", \"eventType\", \"alertStatus\", \"application\", \"customerId\", \"userId\", \"timestamp\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/json-schema/saas-alerts-security-event-schema.json
tags:
- MSP
- SaaS Security
- Security Monitoring
- Threat Detection
- Microsoft 365
- Google Workspace
- MSSP
title: SaaS Alerts Security Event
---
