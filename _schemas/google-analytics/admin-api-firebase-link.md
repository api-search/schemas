---
description: A link between a GA4 property and a Firebase project.
layout: schema
name: FirebaseLink
properties_list:
- description: Output only. Time when this FirebaseLink was originally created.
  name: createTime
  type: string
- description: 'Output only. Example format: properties/1234/firebaseLinks/5678'
  name: name
  type: string
- description: Immutable. Firebase project resource name. When creating a FirebaseLink, you may provide this resource name using either a project number or project ID. Once this resource has been created, returned F
  name: project
  type: string
provider_name: Google Analytics
provider_slug: google-analytics
schema_file: json-schema/admin-api-firebase-link-schema.json
slug: admin-api-firebase-link
source_filename: admin-api-firebase-link-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-firebase-link-schema.json\",\n  \"title\": \"FirebaseLink\",\n  \"description\": \"A link between a GA4 property and a Firebase project.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"createTime\": {\n      \"description\": \"Output only. Time when this FirebaseLink was originally created.\",\n      \"format\": \"google-datetime\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Output only. Example format: properties/1234/firebaseLinks/5678\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"project\": {\n      \"description\": \"Immutable. Firebase project resource name. When creating a FirebaseLink, you may provide this resource name using either a project number or project ID. Once this resource has been\
  \ created, returned FirebaseLinks will always have a project_name that contains a project number. Format: 'projects/{project number}' Example: 'projects/1234'\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-analytics/refs/heads/main/json-schema/admin-api-firebase-link-schema.json
tags:
- Analytics
- Data
- Google
- Metrics
- Reporting
- Web Analytics
- Machine Learning
- Attribution
title: FirebaseLink
---
