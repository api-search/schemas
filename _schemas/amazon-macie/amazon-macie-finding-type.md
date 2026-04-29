---
description: 'The type of finding. For details about each type, see <a href="https://docs.aws.amazon.com/macie/latest/user/findings-types.html">Types of Amazon Macie findings</a> in the <i>Amazon Macie User Guide</i>. Possible values are:'
layout: schema
name: FindingType
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-finding-type-schema.json
slug: amazon-macie-finding-type
source_filename: amazon-macie-finding-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-type-schema.json\",\n  \"title\": \"FindingType\",\n  \"description\": \"The type of finding. For details about each type, see <a href=\\\"https://docs.aws.amazon.com/macie/latest/user/findings-types.html\\\">Types of Amazon Macie findings</a> in the <i>Amazon Macie User Guide</i>. Possible values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"SensitiveData:S3Object/Multiple\",\n    \"SensitiveData:S3Object/Financial\",\n    \"SensitiveData:S3Object/Personal\",\n    \"SensitiveData:S3Object/Credentials\",\n    \"SensitiveData:S3Object/CustomIdentifier\",\n    \"Policy:IAMUser/S3BucketPublic\",\n    \"Policy:IAMUser/S3BucketSharedExternally\",\n    \"Policy:IAMUser/S3BucketReplicatedExternally\",\n    \"Policy:IAMUser/S3BucketEncryptionDisabled\",\n    \"Policy:IAMUser/S3BlockPublicAccessDisabled\"\
  ,\n    \"Policy:IAMUser/S3BucketSharedWithCloudFront\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-type-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: FindingType
---
