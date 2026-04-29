---
description: Represents a Google Tag Manager Trigger. A trigger defines conditions under which tags should fire, such as page views, clicks, form submissions, or custom events.
layout: schema
name: Trigger
properties_list:
- description: GTM Trigger's API relative path.
  name: path
  type: string
- description: GTM Account ID.
  name: accountId
  type: string
- description: GTM Container ID.
  name: containerId
  type: string
- description: GTM Workspace ID.
  name: workspaceId
  type: string
- description: The Trigger ID uniquely identifies the GTM Trigger.
  name: triggerId
  type: string
- description: Trigger display name.
  name: name
  type: string
- description: Defines the data layer event that causes this trigger.
  name: type
  type: string
- description: Used in the case of custom event, which is fired if and only if all Conditions are true.
  name: customEventFilter
  type: array
- description: The trigger will only fire if and only if all Conditions are true.
  name: filter
  type: array
- description: Used in the case of auto event tracking for filtering events.
  name: autoEventFilter
  type: array
- description: The fingerprint of the GTM Trigger as computed at storage time. This value is recomputed whenever the trigger is modified.
  name: fingerprint
  type: string
- description: Parent folder ID.
  name: parentFolderId
  type: string
- description: Auto-generated link to the tag manager UI.
  name: tagManagerUrl
  type: string
- description: User notes on how to apply this trigger in the container.
  name: notes
  type: string
- description: Additional parameters for the trigger.
  name: parameter
  type: array
provider_name: Google Tag Manager
provider_slug: google-tag-manager
schema_file: json-schema/google-tag-manager-v2-trigger-schema.json
slug: google-tag-manager-v2-trigger
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Trigger\",\n  \"type\": \"object\",\n  \"description\": \"Represents a Google Tag Manager Trigger. A trigger defines conditions under which tags should fire, such as page views, clicks, form submissions, or custom events.\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Trigger's API relative path.\"\n    },\n    \"accountId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Account ID.\"\n    },\n    \"containerId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Container ID.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"GTM Workspace ID.\"\n    },\n    \"triggerId\": {\n      \"type\": \"string\",\n      \"description\": \"The Trigger ID uniquely identifies the GTM Trigger.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Trigger display\
  \ name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Defines the data layer event that causes this trigger.\"\n    },\n    \"customEventFilter\": {\n      \"type\": \"array\",\n      \"description\": \"Used in the case of custom event, which is fired if and only if all Conditions are true.\"\n    },\n    \"filter\": {\n      \"type\": \"array\",\n      \"description\": \"The trigger will only fire if and only if all Conditions are true.\"\n    },\n    \"autoEventFilter\": {\n      \"type\": \"array\",\n      \"description\": \"Used in the case of auto event tracking for filtering events.\"\n    },\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"description\": \"The fingerprint of the GTM Trigger as computed at storage time. This value is recomputed whenever the trigger is modified.\"\n    },\n    \"parentFolderId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent folder ID.\"\n    },\n    \"tagManagerUrl\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Auto-generated link to the tag manager UI.\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"description\": \"User notes on how to apply this trigger in the container.\"\n    },\n    \"parameter\": {\n      \"type\": \"array\",\n      \"description\": \"Additional parameters for the trigger.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-tag-manager/refs/heads/main/json-schema/google-tag-manager-v2-trigger-schema.json
tags:
- Analytics
- Conversion Tracking
- Marketing
- Tag Management
- Tracking
title: Trigger
---
