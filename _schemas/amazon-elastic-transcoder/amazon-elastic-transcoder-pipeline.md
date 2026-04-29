---
description: The pipeline (queue) that is used to manage jobs.
layout: schema
name: Pipeline
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: InputBucket
  type: object
- description: ''
  name: OutputBucket
  type: object
- description: ''
  name: Role
  type: object
- description: ''
  name: AwsKmsKeyArn
  type: object
- description: ''
  name: Notifications
  type: object
- description: ''
  name: ContentConfig
  type: object
- description: ''
  name: ThumbnailConfig
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-pipeline-schema.json
slug: amazon-elastic-transcoder-pipeline
source_filename: amazon-elastic-transcoder-pipeline-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-pipeline-schema.json\",\n  \"title\": \"Pipeline\",\n  \"description\": \"The pipeline (queue) that is used to manage jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The identifier for the pipeline. You use this value to identify the pipeline in which you want to perform a variety of operations, such as creating a job or a preset.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the pipeline.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The name of the pipeline. We recommend that the name be unique within the AWS account, but uniqueness is not enforced.</p> <p>Constraints: Maximum 40 characters</p>\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineStatus\"\n        },\n        {\n          \"description\": \"<p>The current status of the pipeline:</p> <ul> <li> <p> <code>Active</code>: The pipeline is processing jobs.</p> </li> <li> <p> <code>Paused</code>: The pipeline is not currently processing jobs.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"InputBucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket from which Elastic Transcoder gets media files for transcoding and the graphics files,\
  \ if any, that you want to use for watermarks.\"\n        }\n      ]\n    },\n    \"OutputBucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket in which you want Elastic Transcoder to save transcoded files, thumbnails, and playlists. Either you specify this value, or you specify both <code>ContentConfig</code> and <code>ThumbnailConfig</code>.\"\n        }\n      ]\n    },\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The IAM Amazon Resource Name (ARN) for the role that Elastic Transcoder uses to transcode jobs for this pipeline.\"\n        }\n      ]\n    },\n    \"AwsKmsKeyArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KeyArn\"\n        },\n        {\n          \"description\": \"<p>The AWS Key Management Service (AWS KMS) key\
  \ that you want to use with this pipeline.</p> <p>If you use either <code>s3</code> or <code>s3-aws-kms</code> as your <code>Encryption:Mode</code>, you don't need to provide a key with your job because a default key, known as an AWS-KMS key, is created for you automatically. You need to provide an AWS-KMS key only if you want to use a non-default AWS-KMS key, or if you are using an <code>Encryption:Mode</code> of <code>aes-cbc-pkcs7</code>, <code>aes-ctr</code>, or <code>aes-gcm</code>.</p>\"\n        }\n      ]\n    },\n    \"Notifications\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notifications\"\n        },\n        {\n          \"description\": \"<p>The Amazon Simple Notification Service (Amazon SNS) topic that you want to notify to report job status.</p> <important> <p>To receive notifications, you must also subscribe to the new topic in the Amazon SNS console.</p> </important> <ul> <li> <p> <b>Progressing</b> (optional): The Amazon Simple Notification\
  \ Service (Amazon SNS) topic that you want to notify when Elastic Transcoder has started to process the job.</p> </li> <li> <p> <b>Complete</b> (optional): The Amazon SNS topic that you want to notify when Elastic Transcoder has finished processing the job.</p> </li> <li> <p> <b>Warning</b> (optional): The Amazon SNS topic that you want to notify when Elastic Transcoder encounters a warning condition.</p> </li> <li> <p> <b>Error</b> (optional): The Amazon SNS topic that you want to notify when Elastic Transcoder encounters an error condition.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ContentConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineOutputConfig\"\n        },\n        {\n          \"description\": \"<p>Information about the Amazon S3 bucket in which you want Elastic Transcoder to save transcoded files and playlists. Either you specify both <code>ContentConfig</code> and <code>ThumbnailConfig</code>, or you specify <code>OutputBucket</code>.</p>\
  \ <ul> <li> <p> <b>Bucket</b>: The Amazon S3 bucket in which you want Elastic Transcoder to save transcoded files and playlists.</p> </li> <li> <p> <b>Permissions</b>: A list of the users and/or predefined Amazon S3 groups you want to have access to transcoded files and playlists, and the type of access that you want them to have. </p> <ul> <li> <p>GranteeType: The type of value that appears in the <code>Grantee</code> object: </p> <ul> <li> <p> <code>Canonical</code>: Either the canonical user ID for an AWS account or an origin access identity for an Amazon CloudFront distribution.</p> </li> <li> <p> <code>Email</code>: The registered email address of an AWS account.</p> </li> <li> <p> <code>Group</code>: One of the following predefined Amazon S3 groups: <code>AllUsers</code>, <code>AuthenticatedUsers</code>, or <code>LogDelivery</code>.</p> </li> </ul> </li> <li> <p> <code>Grantee</code>: The AWS user or group that you want to have access to transcoded files and playlists.</p> </li>\
  \ <li> <p> <code>Access</code>: The permission that you want to give to the AWS user that is listed in <code>Grantee</code>. Valid values include:</p> <ul> <li> <p> <code>READ</code>: The grantee can read the objects and metadata for objects that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>READ_ACP</code>: The grantee can read the object ACL for objects that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>WRITE_ACP</code>: The grantee can write the ACL for the objects that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>FULL_CONTROL</code>: The grantee has <code>READ</code>, <code>READ_ACP</code>, and <code>WRITE_ACP</code> permissions for the objects that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> </ul> </li> </ul> </li> <li> <p> <b>StorageClass</b>: The Amazon S3 storage class, Standard or ReducedRedundancy, that you want Elastic Transcoder to assign to the video files and playlists that\
  \ it stores in your Amazon S3 bucket. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"ThumbnailConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineOutputConfig\"\n        },\n        {\n          \"description\": \"<p>Information about the Amazon S3 bucket in which you want Elastic Transcoder to save thumbnail files. Either you specify both <code>ContentConfig</code> and <code>ThumbnailConfig</code>, or you specify <code>OutputBucket</code>.</p> <ul> <li> <p> <code>Bucket</code>: The Amazon S3 bucket in which you want Elastic Transcoder to save thumbnail files. </p> </li> <li> <p> <code>Permissions</code>: A list of the users and/or predefined Amazon S3 groups you want to have access to thumbnail files, and the type of access that you want them to have. </p> <ul> <li> <p>GranteeType: The type of value that appears in the Grantee object:</p> <ul> <li> <p> <code>Canonical</code>: Either the canonical user ID for an AWS account or an origin\
  \ access identity for an Amazon CloudFront distribution.</p> <important> <p>A canonical user ID is not the same as an AWS account number.</p> </important> </li> <li> <p> <code>Email</code>: The registered email address of an AWS account.</p> </li> <li> <p> <code>Group</code>: One of the following predefined Amazon S3 groups: <code>AllUsers</code>, <code>AuthenticatedUsers</code>, or <code>LogDelivery</code>.</p> </li> </ul> </li> <li> <p> <code>Grantee</code>: The AWS user or group that you want to have access to thumbnail files.</p> </li> <li> <p>Access: The permission that you want to give to the AWS user that is listed in Grantee. Valid values include: </p> <ul> <li> <p> <code>READ</code>: The grantee can read the thumbnails and metadata for thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>READ_ACP</code>: The grantee can read the object ACL for thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>WRITE_ACP</code>:\
  \ The grantee can write the ACL for the thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>FULL_CONTROL</code>: The grantee has READ, READ_ACP, and WRITE_ACP permissions for the thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> </ul> </li> </ul> </li> <li> <p> <code>StorageClass</code>: The Amazon S3 storage class, <code>Standard</code> or <code>ReducedRedundancy</code>, that you want Elastic Transcoder to assign to the thumbnails that it stores in your Amazon S3 bucket.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-pipeline-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: Pipeline
---
