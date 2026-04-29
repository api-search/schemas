---
description: The <code>Permission</code> structure.
layout: schema
name: Permission
properties_list:
- description: ''
  name: GranteeType
  type: object
- description: ''
  name: Grantee
  type: object
- description: ''
  name: Access
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-permission-schema.json
slug: amazon-elastic-transcoder-permission
source_filename: amazon-elastic-transcoder-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-permission-schema.json\",\n  \"title\": \"Permission\",\n  \"description\": \"The <code>Permission</code> structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GranteeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GranteeType\"\n        },\n        {\n          \"description\": \"<p>The type of value that appears in the Grantee object:</p> <ul> <li> <p> <code>Canonical</code>: Either the canonical user ID for an AWS account or an origin access identity for an Amazon CloudFront distribution.</p> <important> <p>A canonical user ID is not the same as an AWS account number.</p> </important> </li> <li> <p> <code>Email</code>: The registered email address of an AWS account.</p> </li> <li> <p> <code>Group</code>: One of the\
  \ following predefined Amazon S3 groups: <code>AllUsers</code>, <code>AuthenticatedUsers</code>, or <code>LogDelivery</code>.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Grantee\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Grantee\"\n        },\n        {\n          \"description\": \"The AWS user or group that you want to have access to transcoded files and playlists. To identify the user or group, you can specify the canonical user ID for an AWS account, an origin access identity for a CloudFront distribution, the registered email address of an AWS account, or a predefined Amazon S3 group.\"\n        }\n      ]\n    },\n    \"Access\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessControls\"\n        },\n        {\n          \"description\": \"<p> The permission that you want to give to the AWS user that is listed in Grantee. Valid values include: </p> <ul> <li> <p> <code>READ</code>: The grantee can read\
  \ the thumbnails and metadata for thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>READ_ACP</code>: The grantee can read the object ACL for thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>WRITE_ACP</code>: The grantee can write the ACL for the thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> <li> <p> <code>FULL_CONTROL</code>: The grantee has READ, READ_ACP, and WRITE_ACP permissions for the thumbnails that Elastic Transcoder adds to the Amazon S3 bucket.</p> </li> </ul>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-permission-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: Permission
---
