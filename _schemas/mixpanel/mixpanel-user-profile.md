---
description: Represents a user profile in Mixpanel People, storing persistent properties about a user such as demographics, preferences, and engagement metrics.
layout: schema
name: Mixpanel User Profile
properties_list:
- description: Unique identifier for the user
  name: $distinct_id
  type: string
- description: User profile properties
  name: $properties
  type: object
provider_name: Mixpanel
provider_slug: mixpanel
schema_file: json-schema/mixpanel-user-profile-schema.json
slug: mixpanel-user-profile
source_filename: mixpanel-user-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developer.mixpanel.com/schemas/mixpanel/user-profile.json\",\n  \"title\": \"Mixpanel User Profile\",\n  \"description\": \"Represents a user profile in Mixpanel People, storing persistent properties about a user such as demographics, preferences, and engagement metrics.\",\n  \"type\": \"object\",\n  \"required\": [\"$distinct_id\"],\n  \"properties\": {\n    \"$distinct_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user\"\n    },\n    \"$properties\": {\n      \"type\": \"object\",\n      \"description\": \"User profile properties\",\n      \"properties\": {\n        \"$first_name\": {\n          \"type\": \"string\",\n          \"description\": \"User's first name\"\n        },\n        \"$last_name\": {\n          \"type\": \"string\",\n          \"description\": \"User's last name\"\n        },\n        \"$name\": {\n          \"type\": \"\
  string\",\n          \"description\": \"User's full name\"\n        },\n        \"$email\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"User's email address\"\n        },\n        \"$phone\": {\n          \"type\": \"string\",\n          \"description\": \"User's phone number\"\n        },\n        \"$avatar\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the user's avatar image\"\n        },\n        \"$city\": {\n          \"type\": \"string\",\n          \"description\": \"User's city\"\n        },\n        \"$region\": {\n          \"type\": \"string\",\n          \"description\": \"User's region or state\"\n        },\n        \"$country_code\": {\n          \"type\": \"string\",\n          \"description\": \"Two-letter country code\"\n        },\n        \"$timezone\": {\n          \"type\": \"string\",\n          \"description\": \"User's timezone (e.g., US/Eastern)\"\
  \n        },\n        \"$created\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the user profile was first created\"\n        },\n        \"$last_seen\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When the user was last active\"\n        }\n      },\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/mixpanel/refs/heads/main/json-schema/mixpanel-user-profile-schema.json
tags:
- Analytics
- Data Analysis
- Event Tracking
- Product Analytics
- User Behavior
title: Mixpanel User Profile
---
