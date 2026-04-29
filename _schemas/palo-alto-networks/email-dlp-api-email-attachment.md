---
description: EmailAttachment schema from Palo Alto Networks Email DLP API
layout: schema
name: EmailAttachment
properties_list:
- description: Attachment filename.
  name: filename
  type: string
- description: MIME content type of the attachment.
  name: content_type
  type: string
- description: Attachment size in bytes.
  name: size
  type: integer
- description: Whether the attachment contained data pattern matches.
  name: has_matches
  type: boolean
- description: Number of data pattern matches in the attachment.
  name: match_count
  type: integer
- description: Names of data patterns that matched in the attachment.
  name: patterns_matched
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/email-dlp-api-email-attachment-schema.json
slug: email-dlp-api-email-attachment
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmailAttachment\",\n  \"description\": \"EmailAttachment schema from Palo Alto Networks Email DLP API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/email-dlp-api-email-attachment-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filename\": {\n      \"type\": \"string\",\n      \"description\": \"Attachment filename.\"\n    },\n    \"content_type\": {\n      \"type\": \"string\",\n      \"description\": \"MIME content type of the attachment.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Attachment size in bytes.\"\n    },\n    \"has_matches\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the attachment contained data pattern matches.\"\n    },\n    \"match_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of data pattern matches\
  \ in the attachment.\"\n    },\n    \"patterns_matched\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Names of data patterns that matched in the attachment.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/email-dlp-api-email-attachment-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: EmailAttachment
---
