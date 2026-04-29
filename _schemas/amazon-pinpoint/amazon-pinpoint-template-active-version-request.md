---
description: Specifies which version of a message template to use as the active version of the template.
layout: schema
name: TemplateActiveVersionRequest
properties_list:
- description: ''
  name: Version
  type: object
provider_name: Amazon Pinpoint
provider_slug: amazon-pinpoint
schema_file: json-schema/amazon-pinpoint-template-active-version-request-schema.json
slug: amazon-pinpoint-template-active-version-request
source_filename: amazon-pinpoint-template-active-version-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-template-active-version-request-schema.json\",\n  \"title\": \"TemplateActiveVersionRequest\",\n  \"description\": \"Specifies which version of a message template to use as the active version of the template.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The version of the message template to use as the active version of the template. Valid values are: latest, for the most recent version of the template; or, the unique identifier for any existing version of the template. If you specify an identifier, the value must match the identifier for an existing template version. To retrieve a list of versions and version identifiers for\
  \ a template, use the <link  linkend=\\\"templates-template-name-template-type-versions\\\">Template Versions</link> resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-pinpoint/refs/heads/main/json-schema/amazon-pinpoint-template-active-version-request-schema.json
tags:
- AWS
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
title: TemplateActiveVersionRequest
---
