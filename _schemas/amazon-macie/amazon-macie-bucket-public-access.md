---
description: Provides information about the permissions settings that determine whether an S3 bucket is publicly accessible.
layout: schema
name: BucketPublicAccess
properties_list:
- description: ''
  name: effectivePermission
  type: object
- description: ''
  name: permissionConfiguration
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-bucket-public-access-schema.json
slug: amazon-macie-bucket-public-access
source_filename: amazon-macie-bucket-public-access-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-public-access-schema.json\",\n  \"title\": \"BucketPublicAccess\",\n  \"description\": \"Provides information about the permissions settings that determine whether an S3 bucket is publicly accessible.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effectivePermission\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectivePermission\"\n        },\n        {\n          \"description\": \" <p>Specifies whether the bucket is publicly accessible due to the combination of permissions settings that apply to the bucket. Possible values are:</p> <ul><li><p>NOT_PUBLIC - The bucket isn't publicly accessible.</p></li> <li><p>PUBLIC - The bucket is publicly accessible.</p></li> <li><p>UNKNOWN - Amazon Macie can't determine whether the bucket is publicly accessible.</p></li></ul>\"\
  \n        }\n      ]\n    },\n    \"permissionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketPermissionConfiguration\"\n        },\n        {\n          \"description\": \"The account-level and bucket-level permissions settings for the bucket.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-bucket-public-access-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: BucketPublicAccess
---
