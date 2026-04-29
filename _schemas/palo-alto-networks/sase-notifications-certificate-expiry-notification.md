---
description: CertificateExpiryNotification schema from SASE Multitenant Notifications
layout: schema
name: CertificateExpiryNotification
properties_list:
- description: Unique identifier for this notification delivery.
  name: notificationId
  type: string
- description: Notification type identifier.
  name: type
  type: string
- description: Tenant Service Group identifier for the affected tenant.
  name: tsg_id
  type: string
- description: Name of the certificate approaching expiration.
  name: certificateName
  type: string
- description: Certificate serial number.
  name: serialNumber
  type: string
- description: Certificate issuer distinguished name.
  name: issuer
  type: string
- description: Certificate subject distinguished name.
  name: subject
  type: string
- description: Certificate expiration date and time.
  name: expirationDate
  type: string
- description: Number of days remaining until the certificate expires.
  name: daysUntilExpiry
  type: integer
- description: List of SASE services or configurations using this certificate.
  name: usedBy
  type: array
- description: Timestamp when this notification was generated.
  name: timestamp
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-notifications-certificate-expiry-notification-schema.json
slug: sase-notifications-certificate-expiry-notification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateExpiryNotification\",\n  \"description\": \"CertificateExpiryNotification schema from SASE Multitenant Notifications\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-certificate-expiry-notification-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"notificationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for this notification delivery.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"certificate_expiry\"\n      ],\n      \"description\": \"Notification type identifier.\"\n    },\n    \"tsg_id\": {\n      \"type\": \"string\",\n      \"description\": \"Tenant Service Group identifier for the affected tenant.\"\n    },\n    \"certificateName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the\
  \ certificate approaching expiration.\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\",\n      \"description\": \"Certificate serial number.\"\n    },\n    \"issuer\": {\n      \"type\": \"string\",\n      \"description\": \"Certificate issuer distinguished name.\"\n    },\n    \"subject\": {\n      \"type\": \"string\",\n      \"description\": \"Certificate subject distinguished name.\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Certificate expiration date and time.\"\n    },\n    \"daysUntilExpiry\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of days remaining until the certificate expires.\"\n    },\n    \"usedBy\": {\n      \"type\": \"array\",\n      \"description\": \"List of SASE services or configurations using this certificate.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"date-time\",\n      \"description\": \"Timestamp when this notification was generated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-notifications-certificate-expiry-notification-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: CertificateExpiryNotification
---
