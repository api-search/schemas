---
description: 'The type of entity that performed the action on the affected resource. Possible values are:'
layout: schema
name: UserIdentityType
properties_list: []
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-user-identity-type-schema.json
slug: amazon-macie-user-identity-type
source_filename: amazon-macie-user-identity-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-user-identity-type-schema.json\",\n  \"title\": \"UserIdentityType\",\n  \"description\": \"The type of entity that performed the action on the affected resource. Possible values are:\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AssumedRole\",\n    \"IAMUser\",\n    \"FederatedUser\",\n    \"Root\",\n    \"AWSAccount\",\n    \"AWSService\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-user-identity-type-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UserIdentityType
---
