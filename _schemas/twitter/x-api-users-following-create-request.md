---
description: UsersFollowingCreateRequest schema from X API v2
layout: schema
name: UsersFollowingCreateRequest
properties_list:
- description: Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.
  name: target_user_id
  type: string
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-users-following-create-request-schema.json
slug: x-api-users-following-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-users-following-create-request-schema.json\",\n  \"title\": \"UsersFollowingCreateRequest\",\n  \"description\": \"UsersFollowingCreateRequest schema from X API v2\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"target_user_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of this User. This is returned as a string in order to avoid complications with languages and tools that cannot handle large integers.\",\n      \"pattern\": \"^[0-9]{1,19}$\",\n      \"example\": \"2244994945\"\n    }\n  },\n  \"required\": [\n    \"target_user_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-users-following-create-request-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: UsersFollowingCreateRequest
---
