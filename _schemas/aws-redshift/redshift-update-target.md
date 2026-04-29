---
description: A maintenance track that you can switch the current track to.
layout: schema
name: UpdateTarget
properties_list:
- description: ''
  name: MaintenanceTrackName
  type: object
- description: ''
  name: DatabaseVersion
  type: object
- description: ''
  name: SupportedOperations
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-update-target-schema.json
slug: redshift-update-target
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"MaintenanceTrackName\": {},\n    \"DatabaseVersion\": {},\n    \"SupportedOperations\": {}\n  },\n  \"description\": \"A maintenance track that you can switch the current track to.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-update-target-schema.json\",\n  \"title\": \"UpdateTarget\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-update-target-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: UpdateTarget
---
