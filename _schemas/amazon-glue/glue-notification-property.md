---
description: Specifies configuration properties of a notification.
layout: schema
name: NotificationProperty
properties_list:
- description: ''
  name: NotifyDelayAfter
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-notification-property-schema.json
slug: glue-notification-property
source_filename: glue-notification-property-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-notification-property-schema.json\",\n  \"title\": \"NotificationProperty\",\n  \"description\": \"Specifies configuration properties of a notification.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NotifyDelayAfter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NotifyDelayAfter\"\n        },\n        {\n          \"description\": \"After a job run starts, the number of minutes to wait before sending a job run delay notification.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-notification-property-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: NotificationProperty
---
