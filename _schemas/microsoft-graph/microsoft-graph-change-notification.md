---
description: Represents the change notification payload sent by Microsoft Graph to a subscriber's webhook endpoint when a subscribed resource changes. The payload is a changeNotificationCollection containing one or more changeNotification objects. Each notification identifies which subscription triggered it, what resource changed, and the type of change (created, updated, or deleted). Notifications may optionally include encrypted resource data when the subscription was configured with includeResourceData set to true.
layout: schema
name: Microsoft Graph Change Notification
properties_list:
- description: The set of change notifications being delivered in this payload. May contain notifications from multiple subscriptions.
  name: value
  type: array
provider_name: Microsoft Graph
provider_slug: microsoft-graph
schema_file: json-schema/microsoft-graph-change-notification-schema.json
slug: microsoft-graph-change-notification
source_filename: microsoft-graph-change-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-graph/change-notification\",\n  \"title\": \"Microsoft Graph Change Notification\",\n  \"description\": \"Represents the change notification payload sent by Microsoft Graph to a subscriber's webhook endpoint when a subscribed resource changes. The payload is a changeNotificationCollection containing one or more changeNotification objects. Each notification identifies which subscription triggered it, what resource changed, and the type of change (created, updated, or deleted). Notifications may optionally include encrypted resource data when the subscription was configured with includeResourceData set to true.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"value\"\n  ],\n  \"properties\": {\n    \"value\": {\n      \"type\": \"array\",\n      \"description\": \"The set of change notifications being delivered in this payload. May contain notifications from\
  \ multiple subscriptions.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/ChangeNotification\"\n      },\n      \"minItems\": 1\n    }\n  },\n  \"$defs\": {\n    \"ChangeNotification\": {\n      \"type\": \"object\",\n      \"description\": \"A single change notification indicating that a subscribed resource has been created, updated, or deleted.\",\n      \"required\": [\n        \"subscriptionId\",\n        \"subscriptionExpirationDateTime\",\n        \"changeType\",\n        \"resource\",\n        \"tenantId\"\n      ],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for this notification.\"\n        },\n        \"subscriptionId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the subscription that generated this notification.\"\n        },\n        \"subscriptionExpirationDateTime\": {\n          \"type\": \"string\",\n      \
  \    \"format\": \"date-time\",\n          \"description\": \"The expiration date and time of the subscription that generated this notification.\"\n        },\n        \"clientState\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"The value of the clientState property sent in the subscription request. Used to verify notification authenticity.\",\n          \"maxLength\": 255\n        },\n        \"changeType\": {\n          \"type\": \"string\",\n          \"description\": \"The type of change that triggered the notification.\",\n          \"enum\": [\n            \"created\",\n            \"updated\",\n            \"deleted\"\n          ]\n        },\n        \"resource\": {\n          \"type\": \"string\",\n          \"description\": \"The URI of the resource that changed, relative to https://graph.microsoft.com.\",\n          \"examples\": [\n            \"users/87d349ed-44d7-43e1-9a83-5f2406dee5bd\",\n            \"me/messages/AAMkAGI1AABSRIM1AAA=\"\n\
  \          ]\n        },\n        \"resourceData\": {\n          \"$ref\": \"#/$defs/ResourceData\"\n        },\n        \"encryptedContent\": {\n          \"$ref\": \"#/$defs/ChangeNotificationEncryptedContent\"\n        },\n        \"tenantId\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the Microsoft Entra tenant from which the change notification originated.\"\n        }\n      }\n    },\n    \"ResourceData\": {\n      \"type\": \"object\",\n      \"description\": \"Basic information about the resource that triggered the change notification, including the OData type and identifier.\",\n      \"properties\": {\n        \"@odata.type\": {\n          \"type\": \"string\",\n          \"description\": \"The OData entity type of the resource.\",\n          \"examples\": [\n            \"#microsoft.graph.message\",\n            \"#microsoft.graph.user\",\n            \"#microsoft.graph.chatMessage\"\n        \
  \  ]\n        },\n        \"@odata.id\": {\n          \"type\": \"string\",\n          \"description\": \"The OData identifier for the resource instance.\"\n        },\n        \"@odata.etag\": {\n          \"type\": \"string\",\n          \"description\": \"The HTTP entity tag representing the version of the resource.\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the resource that triggered the notification.\"\n        }\n      }\n    },\n    \"ChangeNotificationEncryptedContent\": {\n      \"type\": \"object\",\n      \"description\": \"Encrypted resource data attached to a change notification when the subscription was configured with includeResourceData and an encryption certificate.\",\n      \"required\": [\n        \"data\",\n        \"dataSignature\",\n        \"dataKey\",\n        \"encryptionCertificateId\",\n        \"encryptionCertificateThumbprint\"\n      ],\n      \"properties\": {\n        \"data\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Base64-encoded encrypted data that, when decrypted, produces a JSON string conforming to the resource type indicated by dataType.\"\n        },\n        \"dataSignature\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded HMAC-SHA256 hash of the data for validation.\"\n        },\n        \"dataKey\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded symmetric key generated by Microsoft Graph to encrypt the data value. This key is encrypted with the certificate public key provided during subscription creation.\"\n        },\n        \"encryptionCertificateId\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the certificate used to encrypt the dataKey.\"\n        },\n        \"encryptionCertificateThumbprint\": {\n          \"type\": \"string\",\n          \"description\": \"Base64-encoded thumbprint of the certificate used to encrypt the\
  \ dataKey.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-graph/refs/heads/main/json-schema/microsoft-graph-change-notification-schema.json
tags:
- Azure AD
- Collaboration
- Contacts
- Documents
- Email
- Graph
- Identity
- Microsoft
- Office 365
- Presentations
- Productivity
- Spreadsheets
- T1
- Tasks
title: Microsoft Graph Change Notification
---
