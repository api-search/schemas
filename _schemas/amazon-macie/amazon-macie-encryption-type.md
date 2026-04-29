---
description: 'The server-side encryption algorithm that was used to encrypt an S3 object or is used by default to encrypt objects that are added to an S3 bucket. Possible values are:'
layout: schema
name: EncryptionType
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-encryption-type-schema.json
slug: amazon-macie-encryption-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-encryption-type-schema.json\",\n  \"title\": \"EncryptionType\",\n  \"description\": \"The server-side encryption algorithm that was used to encrypt an S3 object or is used by default to encrypt objects that are added to an S3 bucket. Possible values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"NONE\",\n    \"AES256\",\n    \"aws:kms\",\n    \"UNKNOWN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-encryption-type-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: EncryptionType
---
