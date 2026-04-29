---
description: 'Specifies the type of AWS account permitted to manage VPC endpoints.: <ul> <li>AWS_ACCOUNT: Indicates that the account is owned by an AWS user.</li> <li>AWS_SERVICE: Indicates the the account is owned by an AWS service.</li> </ul>'
layout: schema
name: PrincipalType
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-principal-type-schema.json
slug: openapi-principal-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-principal-type-schema.json\",\n  \"title\": \"PrincipalType\",\n  \"description\": \"Specifies the type of AWS account permitted to manage VPC endpoints.: <ul> <li>AWS_ACCOUNT: Indicates that the account is owned by an AWS user.</li> <li>AWS_SERVICE: Indicates the the account is owned by an AWS service.</li> </ul> \",\n  \"type\": \"string\",\n  \"enum\": [\n    \"AWS_ACCOUNT\",\n    \"AWS_SERVICE\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-principal-type-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: PrincipalType
---
