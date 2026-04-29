---
description: The payload delivered to the webhook endpoint for every Prisma Cloud CSPM alert lifecycle event. Contains all contextual information about the event type, the alert, the violated policy, and the affected cloud resource.
layout: schema
name: AlertPayload
properties_list:
- description: The type of alert lifecycle event that triggered this webhook notification. Identifies whether this is a creation, update, resolution, or dismissal event.
  name: notification_type
  type: string
- description: The unique identifier for the Prisma Cloud alert. Alert IDs are prefixed with 'P-' followed by a numeric sequence, used to reference the alert in Prisma Cloud API operations and the management console
  name: alert_id
  type: string
- description: The current lifecycle status of the alert at the time this webhook notification was dispatched.
  name: alert_status
  type: string
- description: The unique UUID identifier of the Prisma Cloud security policy that was violated and triggered this alert. Can be used to retrieve full policy details via the Prisma Cloud API.
  name: policy_id
  type: string
- description: The human-readable display name of the Prisma Cloud security policy that was violated. Provides immediate context about the nature of the misconfiguration or compliance gap detected.
  name: policy_name
  type: string
- description: The cloud service provider where the violating resource resides. Identifies which cloud environment requires investigation and remediation.
  name: cloud_type
  type: string
- description: The cloud provider account ID, subscription ID, or project ID where the violating resource is deployed. Used to identify the specific cloud account requiring remediation.
  name: account_id
  type: string
- description: The unique identifier of the cloud resource that violated the policy. For AWS resources this is typically an ARN. For Azure resources this is the resource ID path. For GCP resources this is the full r
  name: resource_id
  type: string
- description: The cloud provider service or resource type of the violating resource (e.g., s3, ec2, azure_storage_account, google_storage_bucket). Used to identify the type of infrastructure requiring remediation.
  name: resource_type
  type: string
- description: The severity level of the policy violation as defined by the Prisma Cloud security policy. Drives alert prioritization and notification routing in downstream systems.
  name: severity
  type: string
- description: The ISO 8601 date-time string indicating when this alert event occurred. For created events this is the alert creation time. For resolved or dismissed events this is the time of the status change.
  name: timestamp
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/prisma-cloud-webhooks-alert-payload-schema.json
slug: prisma-cloud-webhooks-alert-payload
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AlertPayload\",\n  \"description\": \"The payload delivered to the webhook endpoint for every Prisma Cloud CSPM alert lifecycle event. Contains all contextual information about the event type, the alert, the violated policy, and the affected cloud resource.\\n\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-webhooks-alert-payload-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notification_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of alert lifecycle event that triggered this webhook notification. Identifies whether this is a creation, update, resolution, or dismissal event.\\n\",\n      \"enum\": [\n        \"alert.created\",\n        \"alert.updated\",\n        \"alert.resolved\",\n        \"alert.dismissed\"\n      ],\n      \"example\": \"alert.created\"\n    },\n\
  \    \"alert_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the Prisma Cloud alert. Alert IDs are prefixed with 'P-' followed by a numeric sequence, used to reference the alert in Prisma Cloud API operations and the management console.\\n\",\n      \"example\": \"P-12345678\"\n    },\n    \"alert_status\": {\n      \"type\": \"string\",\n      \"description\": \"The current lifecycle status of the alert at the time this webhook notification was dispatched.\\n\",\n      \"enum\": [\n        \"open\",\n        \"resolved\",\n        \"dismissed\",\n        \"snoozed\"\n      ],\n      \"example\": \"open\"\n    },\n    \"policy_id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique UUID identifier of the Prisma Cloud security policy that was violated and triggered this alert. Can be used to retrieve full policy details via the Prisma Cloud API.\\n\",\n      \"example\": \"a6b45001-e4af-4b52-ac58-9234a68ef123\"\
  \n    },\n    \"policy_name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name of the Prisma Cloud security policy that was violated. Provides immediate context about the nature of the misconfiguration or compliance gap detected.\\n\",\n      \"example\": \"AWS S3 Bucket Publicly Accessible\"\n    },\n    \"cloud_type\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud service provider where the violating resource resides. Identifies which cloud environment requires investigation and remediation.\\n\",\n      \"enum\": [\n        \"aws\",\n        \"azure\",\n        \"gcp\",\n        \"oci\",\n        \"alibaba_cloud\"\n      ],\n      \"example\": \"aws\"\n    },\n    \"account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider account ID, subscription ID, or project ID where the violating resource is deployed. Used to identify the specific cloud account requiring remediation.\\n\",\n      \"example\"\
  : \"123456789012\"\n    },\n    \"resource_id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the cloud resource that violated the policy. For AWS resources this is typically an ARN. For Azure resources this is the resource ID path. For GCP resources this is the full resource name.\\n\",\n      \"example\": \"arn:aws:s3:::my-public-bucket\"\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"description\": \"The cloud provider service or resource type of the violating resource (e.g., s3, ec2, azure_storage_account, google_storage_bucket). Used to identify the type of infrastructure requiring remediation.\\n\",\n      \"example\": \"s3\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level of the policy violation as defined by the Prisma Cloud security policy. Drives alert prioritization and notification routing in downstream systems.\\n\",\n      \"enum\": [\n        \"informational\"\
  ,\n        \"low\",\n        \"medium\",\n        \"high\",\n        \"critical\"\n      ],\n      \"example\": \"high\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 date-time string indicating when this alert event occurred. For created events this is the alert creation time. For resolved or dismissed events this is the time of the status change.\\n\",\n      \"example\": \"2024-01-15T10:30:00.000Z\"\n    }\n  },\n  \"required\": [\n    \"notification_type\",\n    \"alert_id\",\n    \"alert_status\",\n    \"policy_id\",\n    \"policy_name\",\n    \"cloud_type\",\n    \"account_id\",\n    \"resource_id\",\n    \"resource_type\",\n    \"severity\",\n    \"timestamp\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/prisma-cloud-webhooks-alert-payload-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: AlertPayload
---
