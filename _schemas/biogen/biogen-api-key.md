---
description: A developer API key for accessing Biogen services.
layout: schema
name: ApiKey
properties_list:
- description: Key ID.
  name: id
  type: string
- description: Key display name.
  name: name
  type: string
- description: The API key value (shown once at creation).
  name: key
  type: string
- description: Key status.
  name: status
  type: string
- description: Key creation timestamp.
  name: created_at
  type: string
- description: ''
  name: usage
  type: object
provider_name: Biogen
provider_slug: biogen
schema_file: json-schema/biogen-api-key-schema.json
slug: biogen-api-key
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
title: ApiKey
---
