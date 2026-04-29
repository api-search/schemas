---
description: GetAuthorizationTokenResult schema from Amazon CodeArtifact API
layout: schema
name: GetAuthorizationTokenResult
properties_list:
- description: ''
  name: authorizationToken
  type: object
- description: ''
  name: expiration
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-get-authorization-token-result-schema.json
slug: codeartifact-get-authorization-token-result
source_filename: codeartifact-get-authorization-token-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-get-authorization-token-result-schema.json\",\n  \"title\": \"GetAuthorizationTokenResult\",\n  \"description\": \"GetAuthorizationTokenResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"authorizationToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \" The returned authentication token. \"\n        }\n      ]\n    },\n    \"expiration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \" A timestamp that specifies the date and time the authorization token expires. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-get-authorization-token-result-schema.json
tags:
- Amazon
- AWS
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: GetAuthorizationTokenResult
---
