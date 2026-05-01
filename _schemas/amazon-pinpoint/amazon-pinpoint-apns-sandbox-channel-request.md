---
description: Specifies the status and settings of the APNs (Apple Push Notification service) sandbox channel for an application.
layout: schema
name: APNSSandboxChannelRequest
properties_list:
- description: ''
  name: BundleId
  type: object
- description: ''
  name: Certificate
  type: object
- description: ''
  name: DefaultAuthenticationMethod
  type: object
- description: ''
  name: Enabled
  type: object
- description: ''
  name: PrivateKey
  type: object
- description: ''
  name: TeamId
  type: object
- description: ''
  name: TokenKey
  type: object
- description: ''
  name: TokenKeyId
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-apns-sandbox-channel-request-schema.json
slug: amazon-pinpoint-apns-sandbox-channel-request
source_filename: amazon-pinpoint-apns-sandbox-channel-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-apns-sandbox-channel-request-schema.json\",\n  \"title\": \"APNSSandboxChannelRequest\",\n  \"description\": \"Specifies the status and settings of the APNs (Apple Push Notification service) sandbox channel for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BundleId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The bundle identifier that's assigned to your iOS app. This identifier is used for APNs tokens.\"\n        }\n      ]\n    },\n    \"Certificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The APNs client certificate that you received from Apple, if you want Amazon\
  \ Pinpoint to communicate with the APNs sandbox environment by using an APNs certificate.\"\n        }\n      ]\n    },\n    \"DefaultAuthenticationMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The default authentication method that you want Amazon Pinpoint to use when authenticating with the APNs sandbox environment, key or certificate.\"\n        }\n      ]\n    },\n    \"Enabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether to enable the APNs sandbox channel for the application.\"\n        }\n      ]\n    },\n    \"PrivateKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The private key for the APNs client certificate that you want Amazon Pinpoint to use to communicate\
  \ with the APNs sandbox environment.\"\n        }\n      ]\n    },\n    \"TeamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The identifier that's assigned to your Apple developer account team. This identifier is used for APNs tokens.\"\n        }\n      ]\n    },\n    \"TokenKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The authentication key to use for APNs tokens.\"\n        }\n      ]\n    },\n    \"TokenKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The key identifier that's assigned to your APNs signing key, if you want Amazon Pinpoint to communicate with the APNs sandbox environment by using APNs tokens.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-apns-sandbox-channel-request-schema.json
tags:
- Campaigns
- Communications
- Email
- Marketing
- Messaging
- Push Notifications
- SMS
- Voice
- Customer Engagement
- Segmentation
- Journeys
- Analytics
title: APNSSandboxChannelRequest
---
