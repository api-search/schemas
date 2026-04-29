---
description: Container for setting the versioning state.
layout: schema
name: VersioningConfiguration
properties_list:
- description: The versioning state of the bucket.
  name: Status
  type: string
- description: Specifies whether MFA delete is enabled in the bucket versioning configuration.
  name: MFADelete
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-versioning-configuration-schema.json
slug: amazon-s3-rest-versioning-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersioningConfiguration\",\n  \"type\": \"object\",\n  \"description\": \"Container for setting the versioning state.\",\n  \"properties\": {\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The versioning state of the bucket.\"\n    },\n    \"MFADelete\": {\n      \"type\": \"string\",\n      \"description\": \"Specifies whether MFA delete is enabled in the bucket versioning configuration.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-versioning-configuration-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: VersioningConfiguration
---
