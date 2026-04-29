---
description: Optional. The authentication strategy used to secure the broker. The default is SIMPLE.
layout: schema
name: AuthenticationStrategy
properties_list: []
provider_name: Amazon MQ
provider_slug: amazon-mq
schema_file: json-schema/mq-api-authentication-strategy-schema.json
slug: mq-api-authentication-strategy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-authentication-strategy-schema.json\",\n  \"title\": \"AuthenticationStrategy\",\n  \"description\": \"Optional. The authentication strategy used to secure the broker. The default is SIMPLE.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SIMPLE\",\n    \"LDAP\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mq/refs/heads/main/json-schema/mq-api-authentication-strategy-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: AuthenticationStrategy
---
