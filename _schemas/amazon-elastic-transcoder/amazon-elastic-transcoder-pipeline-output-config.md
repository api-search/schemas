---
description: The <code>PipelineOutputConfig</code> structure.
layout: schema
name: PipelineOutputConfig
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: StorageClass
  type: object
- description: ''
  name: Permissions
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-pipeline-output-config-schema.json
slug: amazon-elastic-transcoder-pipeline-output-config
source_filename: amazon-elastic-transcoder-pipeline-output-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-pipeline-output-config-schema.json\",\n  \"title\": \"PipelineOutputConfig\",\n  \"description\": \"The <code>PipelineOutputConfig</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"<p> The Amazon S3 bucket in which you want Elastic Transcoder to save the transcoded files. Specify this value when all of the following are true:</p> <ul> <li> <p>You want to save transcoded files, thumbnails (if any), and playlists (if any) together in one bucket.</p> </li> <li> <p>You do not want to specify the users or groups who have access to the transcoded files, thumbnails, and playlists.</p> </li> <li> <p>You\
  \ do not want to specify the permissions that Elastic Transcoder grants to the files.</p> </li> <li> <p>You want to associate the transcoded files and thumbnails with the Amazon S3 Standard storage class.</p> </li> </ul> <p>If you want to save transcoded files and playlists in one bucket and thumbnails in another bucket, specify which users can access the transcoded files or the permissions the users have, or change the Amazon S3 storage class, omit OutputBucket and specify values for <code>ContentConfig</code> and <code>ThumbnailConfig</code> instead. </p>\"\n        }\n      ]\n    },\n    \"StorageClass\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageClass\"\n        },\n        {\n          \"description\": \" The Amazon S3 storage class, <code>Standard</code> or <code>ReducedRedundancy</code>, that you want Elastic Transcoder to assign to the video files and playlists that it stores in your Amazon S3 bucket. \"\n        }\n      ]\n    },\n \
  \   \"Permissions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Permissions\"\n        },\n        {\n          \"description\": \"<p>Optional. The <code>Permissions</code> object specifies which users and/or predefined Amazon S3 groups you want to have access to transcoded files and playlists, and the type of access you want them to have. You can grant permissions to a maximum of 30 users and/or predefined Amazon S3 groups.</p> <p>If you include <code>Permissions</code>, Elastic Transcoder grants only the permissions that you specify. It does not grant full permissions to the owner of the role specified by <code>Role</code>. If you want that user to have full control, you must explicitly grant full control to the user.</p> <p> If you omit <code>Permissions</code>, Elastic Transcoder grants full control over the transcoded files and playlists to the owner of the role specified by <code>Role</code>, and grants no other permissions to any other user or group.</p>\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-pipeline-output-config-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: PipelineOutputConfig
---
