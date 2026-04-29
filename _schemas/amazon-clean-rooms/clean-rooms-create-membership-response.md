---
description: Response for creating a membership.
layout: schema
name: CreateMembershipResponse
properties_list:
- description: ''
  name: membership
  type: object
provider_name: Amazon Clean Rooms
provider_slug: amazon-clean-rooms
schema_file: json-schema/clean-rooms-create-membership-response-schema.json
slug: clean-rooms-create-membership-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-membership-response-schema.json\",\n  \"title\": \"CreateMembershipResponse\",\n  \"description\": \"Response for creating a membership.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"membership\": {\n      \"$ref\": \"#/components/schemas/Membership\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-clean-rooms/refs/heads/main/json-schema/clean-rooms-create-membership-response-schema.json
tags:
- AWS
- Clean Rooms
- Data Collaboration
- Privacy
- Analytics
- Marketing
title: CreateMembershipResponse
---
