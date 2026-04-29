---
description: Report email delivery settings.
layout: schema
name: ReportDelivery
properties_list:
- description: Whether the report should be emailed to the report owner.
  name: emailOwner
  type: boolean
- description: The type of delivery for the owner email.
  name: emailOwnerDeliveryType
  type: string
- description: The message to include in the email.
  name: message
  type: string
- description: The list of recipients to send the report to.
  name: recipients
  type: array
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-report-delivery-schema.json
slug: google-campaign-manager-report-delivery
source_filename: google-campaign-manager-report-delivery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ReportDelivery\",\n  \"type\": \"object\",\n  \"description\": \"Report email delivery settings.\",\n  \"properties\": {\n    \"emailOwner\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the report should be emailed to the report owner.\"\n    },\n    \"emailOwnerDeliveryType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of delivery for the owner email.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The message to include in the email.\"\n    },\n    \"recipients\": {\n      \"type\": \"array\",\n      \"description\": \"The list of recipients to send the report to.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-report-delivery-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: ReportDelivery
---
