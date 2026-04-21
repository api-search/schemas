---
description: GetDownloadAuthorizationRequest schema from Backblaze B2 Native API
layout: schema
name: GetDownloadAuthorizationRequest
properties_list:
- description: Bucket to authorize downloads from
  name: bucketId
  type: string
- description: Files must have this name prefix
  name: fileNamePrefix
  type: string
- description: Duration (1 to 604800) the token is valid
  name: validDurationInSeconds
  type: integer
provider_name: Backblaze
provider_slug: backblaze
schema_file: json-schema/b2-native-api-get-download-authorization-request-schema.json
slug: b2-native-api-get-download-authorization-request
tags:
- Cloud Storage
- Object Storage
- Storage
- Backup
title: GetDownloadAuthorizationRequest
---
