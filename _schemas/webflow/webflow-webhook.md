---
description: A Webflow Webhook registration object representing an app-created webhook for a site, as returned by the Webflow Data API v2. Webhooks allow applications to receive real-time notifications when specific events occur on a Webflow site.
layout: schema
name: Webflow Webhook
properties_list:
- description: Unique identifier for the Webhook registration.
  name: id
  type: string
- description: The type of event that triggers the webhook request.
  name: triggerType
  type: string
- description: URL to send the Webhook payload to.
  name: url
  type: string
- description: Unique identifier for the Workspace the Webhook is registered in.
  name: workspaceId
  type: string
- description: Unique identifier for the Site the Webhook is registered in.
  name: siteId
  type: string
- description: Only supported for the form_submission trigger type. Filter for the form you want Webhooks to be sent for.
  name: filter
  type:
  - object
  - 'null'
- description: Date the Webhook instance was last triggered.
  name: lastTriggered
  type: string
- description: Date the Webhook registration was created.
  name: createdOn
  type: string
provider_name: Webflow
provider_slug: webflow
schema_file: json-schema/webflow-webhook-schema.json
slug: webflow-webhook
source_filename: webflow-webhook-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.webflow.com/schemas/webhook.json\",\n  \"title\": \"Webflow Webhook\",\n  \"description\": \"A Webflow Webhook registration object representing an app-created webhook for a site, as returned by the Webflow Data API v2. Webhooks allow applications to receive real-time notifications when specific events occur on a Webflow site.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Unique identifier for the Webhook registration.\",\n      \"examples\": [\"57ca0a9e418c504a6e1acbb6\"]\n    },\n    \"triggerType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of event that triggers the webhook request.\",\n      \"enum\": [\n        \"form_submission\",\n        \"site_publish\",\n        \"page_created\",\n        \"page_metadata_updated\",\n        \"page_deleted\",\n      \
  \  \"ecomm_new_order\",\n        \"ecomm_order_changed\",\n        \"ecomm_inventory_changed\",\n        \"collection_item_created\",\n        \"collection_item_changed\",\n        \"collection_item_deleted\",\n        \"collection_item_published\",\n        \"collection_item_unpublished\",\n        \"comment_created\"\n      ],\n      \"examples\": [\"form_submission\"]\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to send the Webhook payload to.\",\n      \"examples\": [\"https://example.com/webhook\"]\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Unique identifier for the Workspace the Webhook is registered in.\",\n      \"examples\": [\"580e63e98c9a982ac9b8b741\"]\n    },\n    \"siteId\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Unique identifier for the Site the Webhook is registered in.\",\n      \"examples\": [\"562ac0395358780a1f5e6fbd\"\
  ]\n    },\n    \"filter\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"Only supported for the form_submission trigger type. Filter for the form you want Webhooks to be sent for.\",\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the form you'd like to receive notifications for.\",\n          \"examples\": [\"My Form\"]\n        }\n      }\n    },\n    \"lastTriggered\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"description\": \"Date the Webhook instance was last triggered.\",\n      \"examples\": [\"2016-09-06T21:12:22.148Z\"]\n    },\n    \"createdOn\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"description\": \"Date the Webhook registration was created.\",\n      \"examples\": [\"2016-09-02T23:26:22.241Z\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/json-schema/webflow-webhook-schema.json
tags:
- CMS
- Ecommerce
- No-Code
- Web Development
title: Webflow Webhook
---
