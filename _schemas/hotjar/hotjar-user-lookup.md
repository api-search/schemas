---
description: A request to look up or delete user data across sites in a Hotjar organization for GDPR compliance. At least one of data_subject_email or data_subject_site_id_to_user_id_map must be provided.
layout: schema
name: Hotjar User Lookup Request
properties_list:
- description: The email address of the data subject to look up.
  name: data_subject_email
  type: string
- description: A map of site IDs to user IDs on your site, used when user attributes have been sent via the Identify API.
  name: data_subject_site_id_to_user_id_map
  type: object
- description: Whether to immediately delete all found data for the user. Set to true to submit a deletion request.
  name: delete_all_hits
  type: boolean
provider_name: hotjar
provider_slug: hotjar
schema_file: json-schema/hotjar-user-lookup-schema.json
slug: hotjar-user-lookup
source_filename: hotjar-user-lookup-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://hotjar.com/schemas/hotjar/user-lookup.json\",\n  \"title\": \"Hotjar User Lookup Request\",\n  \"description\": \"A request to look up or delete user data across sites in a Hotjar organization for GDPR compliance. At least one of data_subject_email or data_subject_site_id_to_user_id_map must be provided.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data_subject_email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the data subject to look up.\"\n    },\n    \"data_subject_site_id_to_user_id_map\": {\n      \"type\": \"object\",\n      \"description\": \"A map of site IDs to user IDs on your site, used when user attributes have been sent via the Identify API.\",\n      \"additionalProperties\": {\n        \"type\": \"string\",\n        \"description\": \"The user ID on your site associated with the given site ID.\"\
  \n      }\n    },\n    \"delete_all_hits\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to immediately delete all found data for the user. Set to true to submit a deletion request.\",\n      \"default\": false\n    }\n  },\n  \"anyOf\": [\n    { \"required\": [\"data_subject_email\"] },\n    { \"required\": [\"data_subject_site_id_to_user_id_map\"] }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hotjar/refs/heads/main/json-schema/hotjar-user-lookup-schema.json
tags: []
title: Hotjar User Lookup Request
---
