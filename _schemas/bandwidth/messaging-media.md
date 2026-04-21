---
description: Media schema from Bandwidth messaging API
layout: schema
name: Media
properties_list:
- description: The name of the media file
  name: mediaName
  type: string
- description: The size of the media file in bytes
  name: contentLength
  type: integer
- description: The MIME type of the media file
  name: contentType
  type: string
- description: The URL to access the media content
  name: content
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/messaging-media-schema.json
slug: messaging-media
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Media
---
