---
description: Represents a subscription that allows a client application to receive change notifications about changes to data in Microsoft Graph. Applications create subscriptions specifying the resource to monitor, the types of changes to track, and a notification endpoint URL. When changes occur, Microsoft Graph sends HTTP POST notifications to the specified endpoint. Subscriptions have limited lifetimes that vary by resource type and must be renewed before expiration.
layout: schema
name: Microsoft Graph Subscription
properties_list:
- description: Unique identifier for the subscription. Read-only.
  name: id
  type: string
- description: Specifies the resource that is monitored for changes. Do not include the base URL (https://graph.microsoft.com/v1.0/). See the supported resource path values for each resource type.
  name: resource
  type: string
- description: 'Indicates the type of change in the subscribed resource that raises a change notification. The supported values are: created, updated, deleted. Multiple values can be combined using a comma-separated '
  name: changeType
  type: string
- description: The URL of the endpoint that receives the change notifications. This URL must use the HTTPS protocol. Any query string parameter included in the notificationUrl property is included in the HTTP POST r
  name: notificationUrl
  type: string
- description: Required for Teams resources if the expirationDateTime value is more than 1 hour from now; optional otherwise. The URL of the endpoint that receives lifecycle notifications, including subscriptionRemo
  name: lifecycleNotificationUrl
  type:
  - string
  - 'null'
- description: Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to. Any value und
  name: expirationDateTime
  type: string
- description: Specifies the value of the clientState property sent by the service in each change notification. The maximum length is 128 characters. The client can check that the change notification came from the s
  name: clientState
  type:
  - string
  - 'null'
- description: Identifier of the application used to create the subscription. Read-only.
  name: applicationId
  type:
  - string
  - 'null'
- description: Identifier of the user or service principal that created the subscription. If the app used delegated permissions, this field contains the ID of the signed-in user. If application permissions were used
  name: creatorId
  type:
  - string
  - 'null'
- description: When set to true, change notifications include resource data (such as content of a chat message). Requires encryptionCertificate and encryptionCertificateId to be set.
  name: includeResourceData
  type:
  - boolean
  - 'null'
- description: A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications. Required when includeResourceData is true.
  name: encryptionCertificate
  type:
  - string
  - 'null'
- description: A custom app-provided identifier to help identify the certificate needed to decrypt resource data.
  name: encryptionCertificateId
  type:
  - string
  - 'null'
- description: Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint supports.
  name: latestSupportedTlsVersion
  type:
  - string
  - 'null'
- description: OData query options for specifying the value for the targeting resource. Clients receive notifications when the resource reaches the state matching the query options provided here.
  name: notificationQueryOptions
  type:
  - string
  - 'null'
- description: The app ID that the subscription service can use to generate the validation token. The value allows the client to validate the authenticity of the notification received.
  name: notificationUrlAppId
  type:
  - string
  - 'null'
provider_name: Microsoft Graph
provider_slug: microsoft-graph
schema_file: json-schema/microsoft-graph-subscription-schema.json
slug: microsoft-graph-subscription
source_filename: microsoft-graph-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.api.gov/microsoft-graph/subscription\",\n  \"title\": \"Microsoft Graph Subscription\",\n  \"description\": \"Represents a subscription that allows a client application to receive change notifications about changes to data in Microsoft Graph. Applications create subscriptions specifying the resource to monitor, the types of changes to track, and a notification endpoint URL. When changes occur, Microsoft Graph sends HTTP POST notifications to the specified endpoint. Subscriptions have limited lifetimes that vary by resource type and must be renewed before expiration.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"changeType\",\n    \"notificationUrl\",\n    \"resource\",\n    \"expirationDateTime\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the subscription. Read-only.\",\n      \"readOnly\": true,\n\
  \      \"examples\": [\n        \"7f105c7d-2dc5-4530-97cd-4e7ae6534c07\"\n      ]\n    },\n    \"resource\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies the resource that is monitored for changes. Do not include the base URL (https://graph.microsoft.com/v1.0/). See the supported resource path values for each resource type.\",\n      \"examples\": [\n        \"me/mailFolders('Inbox')/messages\",\n        \"users\",\n        \"groups\",\n        \"teams/allMessages\",\n        \"chats/allMessages\"\n      ]\n    },\n    \"changeType\": {\n      \"type\": \"string\",\n      \"description\": \"Indicates the type of change in the subscribed resource that raises a change notification. The supported values are: created, updated, deleted. Multiple values can be combined using a comma-separated list.\",\n      \"examples\": [\n        \"created\",\n        \"updated\",\n        \"deleted\",\n        \"created,updated\",\n        \"created,updated,deleted\"\n      ]\n    },\n\
  \    \"notificationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL of the endpoint that receives the change notifications. This URL must use the HTTPS protocol. Any query string parameter included in the notificationUrl property is included in the HTTP POST request when Microsoft Graph sends the change notifications.\",\n      \"pattern\": \"^https://\"\n    },\n    \"lifecycleNotificationUrl\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"uri\",\n      \"description\": \"Required for Teams resources if the expirationDateTime value is more than 1 hour from now; optional otherwise. The URL of the endpoint that receives lifecycle notifications, including subscriptionRemoved, reauthorizationRequired, and missed notifications. This URL must use the HTTPS protocol.\",\n      \"pattern\": \"^https://\"\n    },\n    \"expirationDateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\"\
  : \"Specifies the date and time when the webhook subscription expires. The time is in UTC, and can be an amount of time from subscription creation that varies for the resource subscribed to. Any value under 45 minutes after the time of the request is automatically set to 45 minutes after the request time.\"\n    },\n    \"clientState\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Specifies the value of the clientState property sent by the service in each change notification. The maximum length is 128 characters. The client can check that the change notification came from the service by comparing the values.\",\n      \"maxLength\": 128\n    },\n    \"applicationId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Identifier of the application used to create the subscription. Read-only.\",\n      \"readOnly\": true\n    },\n    \"creatorId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Identifier of the user or service\
  \ principal that created the subscription. If the app used delegated permissions, this field contains the ID of the signed-in user. If application permissions were used, this contains the service principal ID. Read-only.\",\n      \"readOnly\": true\n    },\n    \"includeResourceData\": {\n      \"type\": [\"boolean\", \"null\"],\n      \"description\": \"When set to true, change notifications include resource data (such as content of a chat message). Requires encryptionCertificate and encryptionCertificateId to be set.\"\n    },\n    \"encryptionCertificate\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A base64-encoded representation of a certificate with a public key used to encrypt resource data in change notifications. Required when includeResourceData is true.\"\n    },\n    \"encryptionCertificateId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"A custom app-provided identifier to help identify the certificate needed to decrypt resource\
  \ data.\"\n    },\n    \"latestSupportedTlsVersion\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Specifies the latest version of Transport Layer Security (TLS) that the notification endpoint supports.\",\n      \"enum\": [\"v1_0\", \"v1_1\", \"v1_2\", \"v1_3\", null]\n    },\n    \"notificationQueryOptions\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"OData query options for specifying the value for the targeting resource. Clients receive notifications when the resource reaches the state matching the query options provided here.\"\n    },\n    \"notificationUrlAppId\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"The app ID that the subscription service can use to generate the validation token. The value allows the client to validate the authenticity of the notification received.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-graph/refs/heads/main/json-schema/microsoft-graph-subscription-schema.json
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
title: Microsoft Graph Subscription
---
