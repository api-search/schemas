---
description: MtNotification schema from Multi-Tenant Notifications API
layout: schema
name: MtNotification
properties_list:
- description: Notification id
  name: id
  type: string
- description: Notification name
  name: name
  type: string
- description: Description of the notification
  name: body
  type: string
- description: Action to be taken on receiving the notification (if applicable)
  name: action
  type: string
- description: Notification creation time
  name: createdTime
  type: number
- description: Multi-Tenant Notification Aggregation Key
  name: aggKey
  type: object
- description: List of impacted tenants
  name: impactedTenants
  type: array
- description: Number of tenants impacted by the multi-tenant notification
  name: impactedTenantCount
  type: number
- description: Read state of the notification
  name: notifReadState
  type: string
- description: List of output channels that the notification is sent on
  name: notifChannels
  type: array
- description: Notification type
  name: notifType
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-mt-notification-schema.json
slug: sase-multitenant-notifications-api-mt-notification
source_filename: sase-multitenant-notifications-api-mt-notification-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MtNotification\",\n  \"description\": \"MtNotification schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-mt-notification-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Notification id\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Notification name\",\n      \"type\": \"string\"\n    },\n    \"body\": {\n      \"description\": \"Description of the notification\",\n      \"type\": \"string\"\n    },\n    \"action\": {\n      \"description\": \"Action to be taken on receiving the notification (if applicable)\",\n      \"type\": \"string\"\n    },\n    \"createdTime\": {\n      \"description\": \"Notification creation time\",\n      \"type\": \"number\"\n    },\n    \"\
  aggKey\": {\n      \"type\": \"object\",\n      \"description\": \"Multi-Tenant Notification Aggregation Key\",\n      \"properties\": {\n        \"tag\": {\n          \"required\": [\n            \"tsgId\",\n            \"notifType\",\n            \"category\",\n            \"subCategory\",\n            \"inAppFlag\"\n          ],\n          \"type\": \"object\",\n          \"properties\": {\n            \"tsgId\": {\n              \"description\": \"TSG Id\",\n              \"type\": \"string\"\n            },\n            \"notifType\": {\n              \"description\": \"Notification Type\",\n              \"type\": \"string\",\n              \"enum\": [\n                \"INCIDENTS\",\n                \"UPGRADES\",\n                \"ANNOUNCEMENTS\"\n              ]\n            },\n            \"category\": {\n              \"description\": \"Notification category - is associated with notification type\",\n              \"type\": \"string\"\n            },\n            \"subCategory\"\
  : {\n              \"description\": \"Notification sub-category - is associated with notification type and notification category\",\n              \"type\": \"string\"\n            },\n            \"inAppFlag\": {\n              \"description\": \"InApp Notification Flag\",\n              \"type\": \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"impactedTenants\": {\n      \"description\": \"List of impacted tenants\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"impactedTenantCount\": {\n      \"description\": \"Number of tenants impacted by the multi-tenant notification\",\n      \"type\": \"number\"\n    },\n    \"notifReadState\": {\n      \"type\": \"string\",\n      \"description\": \"Read state of the notification\",\n      \"enum\": [\n        \"READ\",\n        \"UNREAD\"\n      ]\n    },\n    \"notifChannels\": {\n      \"description\": \"List of output channels that the notification is sent on\"\
  ,\n      \"type\": \"array\",\n      \"items\": {\n        \"required\": [\n          \"name\",\n          \"type\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"description\": \"Notification channel name\",\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"description\": \"Notification channel type\",\n            \"type\": \"string\",\n            \"enum\": [\n              \"EMAIL\",\n              \"WEBHOOK\"\n            ]\n          },\n          \"emailChannelDetails\": {\n            \"description\": \"Email channel details\",\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"required\": [\n                \"emails\"\n              ],\n              \"type\": \"object\",\n              \"properties\": {\n                \"emails\": {\n                  \"description\": \"List of emails\",\n                  \"type\": \"array\",\n         \
  \         \"items\": {\n                    \"required\": [\n                      \"name\",\n                      \"emailId\"\n                    ],\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"name\": {\n                        \"description\": \"Email owner name\",\n                        \"type\": \"string\"\n                      },\n                      \"emailId\": {\n                        \"description\": \"Email id\",\n                        \"type\": \"string\"\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          },\n          \"webhookChannelDetails\": {\n            \"description\": \"Webhook channel details\",\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"required\": [\n                \"urls\",\n                \"authType\",\n                \"token\"\n              ],\n          \
  \    \"type\": \"object\",\n              \"properties\": {\n                \"urls\": {\n                  \"description\": \"List of Webhook URLs - do not include token in the URL\",\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                },\n                \"authType\": {\n                  \"description\": \"Webhook Authentication Type\",\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"NO_AUTH\",\n                    \"TOKEN\"\n                  ]\n                },\n                \"token\": {\n                  \"description\": \"Webhook token value\",\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"template\": {\n            \"description\": \"Channel output template\",\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n   \
  \             \"description\": \"Output channel template name\",\n                \"type\": \"string\"\n              },\n              \"templateJson\": {\n                \"description\": \"JSON describing the output channel template\",\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"notifType\": {\n      \"description\": \"Notification type\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"body\",\n    \"aggKey\",\n    \"notifReadState\",\n    \"impactedTenants\",\n    \"impactedTenantCount\",\n    \"notifChannels\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-mt-notification-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: MtNotification
---
