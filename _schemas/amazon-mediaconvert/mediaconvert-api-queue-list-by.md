---
description: Optional. When you request a list of queues, you can choose to list them alphabetically by NAME or chronologically by CREATION_DATE. If you don't specify, the service will list them by creation date.
layout: schema
name: QueueListBy
properties_list: []
provider_name: Amazon MediaConvert
provider_slug: amazon-mediaconvert
schema_file: json-schema/mediaconvert-api-queue-list-by-schema.json
slug: mediaconvert-api-queue-list-by
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-list-by-schema.json\",\n  \"title\": \"QueueListBy\",\n  \"description\": \"Optional. When you request a list of queues, you can choose to list them alphabetically by NAME or chronologically by CREATION_DATE. If you don't specify, the service will list them by creation date.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NAME\",\n    \"CREATION_DATE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediaconvert/refs/heads/main/json-schema/mediaconvert-api-queue-list-by-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: QueueListBy
---
