---
description: NotifProfile schema from Multi-Tenant Notifications API
layout: schema
name: NotifProfile
properties_list:
- description: Notification Profile Id
  name: id
  type: string
- description: Notification Profile Name
  name: profileName
  type: string
- description: Notification Profile Description
  name: description
  type: string
- description: Notification Profile Operational State
  name: opState
  type: string
- description: Notification Profile Status
  name: status
  type: string
- description: Input Tenant List
  name: tenantList
  type: array
- description: List of excluded tenants
  name: excludeTenantList
  type: array
- description: Notification Type Detail
  name: notifTypeDetails
  type: array
- description: Notification Channel List
  name: notifChannels
  type: array
- description: List of child tenants that got the incident profile
  name: successTenant
  type: array
- description: List of child tenants that didn't get the incident profile
  name: failureTenant
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-notifications-api-notif-profile-schema.json
slug: sase-multitenant-notifications-api-notif-profile
source_filename: sase-multitenant-notifications-api-notif-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NotifProfile\",\n  \"description\": \"NotifProfile schema from Multi-Tenant Notifications API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-profile-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"Notification Profile Id\",\n      \"type\": \"string\"\n    },\n    \"profileName\": {\n      \"description\": \"Notification Profile Name\",\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"description\": \"Notification Profile Description\",\n      \"type\": \"string\"\n    },\n    \"opState\": {\n      \"description\": \"Notification Profile Operational State\",\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ]\n    },\n    \"status\": {\n      \"description\": \"Notification\
  \ Profile Status\",\n      \"type\": \"string\"\n    },\n    \"tenantList\": {\n      \"description\": \"Input Tenant List\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"excludeTenantList\": {\n      \"description\": \"List of excluded tenants\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"notifTypeDetails\": {\n      \"description\": \"Notification Type Detail\",\n      \"type\": \"array\",\n      \"items\": {\n        \"required\": [\n          \"type\",\n          \"notifCategoryList\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"description\": \"Notification Type\",\n            \"type\": \"string\",\n            \"enum\": [\n              \"INCIDENTS\",\n              \"UPGRADES\",\n              \"ANNOUNCEMENTS\"\n            ]\n          },\n          \"notifCategoryList\": {\n            \"description\"\
  : \"List of notification type categories\",\n            \"type\": \"array\",\n            \"items\": {\n              \"required\": [\n                \"name\",\n                \"bestPractice\",\n                \"subCategoryList\"\n              ],\n              \"type\": \"object\",\n              \"properties\": {\n                \"name\": {\n                  \"description\": \"Notification type category name\",\n                  \"type\": \"string\"\n                },\n                \"bestPractice\": {\n                  \"description\": \"Best practice flag for category\",\n                  \"type\": \"boolean\"\n                },\n                \"subCategoryList\": {\n                  \"description\": \"List of notification type sub-categories\",\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"required\": [\n                      \"name\",\n                      \"bestPractice\",\n                      \"needLicense\"\n\
  \                    ],\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"name\": {\n                        \"description\": \"Notification type sub-category name\",\n                        \"type\": \"string\"\n                      },\n                      \"bestPractice\": {\n                        \"description\": \"Best practice flag for sub-category\",\n                        \"type\": \"boolean\"\n                      },\n                      \"needLicense\": {\n                        \"description\": \"Need license flag for sub-category\",\n                        \"type\": \"boolean\"\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"notifChannels\": {\n      \"description\": \"Notification Channel List\",\n      \"type\": \"array\",\n      \"items\": {\n        \"required\": [\n          \"name\"\
  ,\n          \"type\"\n        ],\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"description\": \"Notification channel name\",\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"description\": \"Notification channel type\",\n            \"type\": \"string\",\n            \"enum\": [\n              \"EMAIL\",\n              \"WEBHOOK\"\n            ]\n          },\n          \"emailChannelDetails\": {\n            \"description\": \"Email channel details\",\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"required\": [\n                \"emails\"\n              ],\n              \"type\": \"object\",\n              \"properties\": {\n                \"emails\": {\n                  \"description\": \"List of emails\",\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"required\": [\n                      \"name\",\n \
  \                     \"emailId\"\n                    ],\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"name\": {\n                        \"description\": \"Email owner name\",\n                        \"type\": \"string\"\n                      },\n                      \"emailId\": {\n                        \"description\": \"Email id\",\n                        \"type\": \"string\"\n                      }\n                    }\n                  }\n                }\n              }\n            }\n          },\n          \"webhookChannelDetails\": {\n            \"description\": \"Webhook channel details\",\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"required\": [\n                \"urls\",\n                \"authType\",\n                \"token\"\n              ],\n              \"type\": \"object\",\n              \"properties\": {\n                \"urls\": {\n     \
  \             \"description\": \"List of Webhook URLs - do not include token in the URL\",\n                  \"type\": \"array\",\n                  \"items\": {\n                    \"type\": \"string\"\n                  }\n                },\n                \"authType\": {\n                  \"description\": \"Webhook Authentication Type\",\n                  \"type\": \"string\",\n                  \"enum\": [\n                    \"NO_AUTH\",\n                    \"TOKEN\"\n                  ]\n                },\n                \"token\": {\n                  \"description\": \"Webhook token value\",\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"template\": {\n            \"description\": \"Channel output template\",\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"description\": \"Output channel template name\",\n                \"type\": \"string\"\
  \n              },\n              \"templateJson\": {\n                \"description\": \"JSON describing the output channel template\",\n                \"type\": \"string\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"successTenant\": {\n      \"description\": \"List of child tenants that got the incident profile\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"failureTenant\": {\n      \"description\": \"List of child tenants that didn't get the incident profile\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"profileName\",\n    \"opState\",\n    \"status\",\n    \"tenantList\",\n    \"notifTypeDetails\",\n    \"notifChannels\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-notifications-api-notif-profile-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: NotifProfile
---
