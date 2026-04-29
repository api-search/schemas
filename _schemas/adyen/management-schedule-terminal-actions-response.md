---
description: ScheduleTerminalActionsResponse schema from Adyen API
layout: schema
name: ScheduleTerminalActionsResponse
properties_list:
- description: Information about the action to take.
  name: actionDetails
  type: object
- description: A list containing a terminal ID and an action ID for each terminal that the action was scheduled for.
  name: items
  type: array
- description: 'The date and time when the action should happen. Format: [RFC 3339](https://www.rfc-editor.org/rfc/rfc3339), but without the **Z** before the time offset. For example, **2021-11-15T12:16:21+01:00** Th'
  name: scheduledAt
  type: string
- description: The unique ID of the [store](https://docs.adyen.com/api-explorer/#/ManagementService/latest/get/stores). If present, all terminals in the `terminalIds` list must be assigned to this store.
  name: storeId
  type: string
- description: The validation errors that occurred in the list of terminals, and for each error the IDs of the terminals that the error applies to.
  name: terminalsWithErrors
  type: object
- description: The number of terminals for which scheduling the action failed.
  name: totalErrors
  type: integer
- description: The number of terminals for which the action was successfully scheduled. This doesn't mean the action has happened yet.
  name: totalScheduled
  type: integer
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-schedule-terminal-actions-response-schema.json
slug: management-schedule-terminal-actions-response
source_filename: management-schedule-terminal-actions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-schedule-terminal-actions-response-schema.json\",\n  \"title\": \"ScheduleTerminalActionsResponse\",\n  \"description\": \"ScheduleTerminalActionsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionDetails\": {\n      \"description\": \"Information about the action to take.\",\n      \"oneOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstallAndroidAppDetails\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/InstallAndroidCertificateDetails\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/ReleaseUpdateDetails\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/UninstallAndroidAppDetails\"\n        },\n        {\n          \"$ref\": \"#/components/schemas/UninstallAndroidCertificateDetails\"\
  \n        }\n      ]\n    },\n    \"items\": {\n      \"x-addedInVersion\": \"1\",\n      \"description\": \"A list containing a terminal ID and an action ID for each terminal that the action was scheduled for.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TerminalActionScheduleDetail\"\n      },\n      \"type\": \"array\"\n    },\n    \"scheduledAt\": {\n      \"description\": \"The date and time when the action should happen. \\nFormat: [RFC 3339](https://www.rfc-editor.org/rfc/rfc3339), but without the **Z** before the time offset. For example, **2021-11-15T12:16:21+01:00** \\nThe action is sent with the first [maintenance call](https://docs.adyen.com/point-of-sale/automating-terminal-management/terminal-actions-api#when-actions-take-effect) after the specified date and time in the time zone of the terminal. \\nAn empty value causes the action to be sent as soon as possible: at the next maintenance call.\",\n      \"type\": \"string\"\n    },\n    \"storeId\": {\n\
  \      \"description\": \"The unique ID of the [store](https://docs.adyen.com/api-explorer/#/ManagementService/latest/get/stores). If present, all terminals in the `terminalIds` list must be assigned to this store.\",\n      \"type\": \"string\"\n    },\n    \"terminalsWithErrors\": {\n      \"additionalProperties\": {\n        \"items\": {\n          \"type\": \"string\"\n        },\n        \"type\": \"array\"\n      },\n      \"description\": \"The validation errors that occurred in the list of terminals, and for each error the IDs of the terminals that the error applies to.\",\n      \"type\": \"object\"\n    },\n    \"totalErrors\": {\n      \"description\": \"The number of terminals for which scheduling the action failed.\",\n      \"format\": \"int32\",\n      \"type\": \"integer\"\n    },\n    \"totalScheduled\": {\n      \"description\": \"The number of terminals for which the action was successfully scheduled. This doesn't mean the action has happened yet.\",\n      \"format\"\
  : \"int32\",\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-schedule-terminal-actions-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ScheduleTerminalActionsResponse
---
