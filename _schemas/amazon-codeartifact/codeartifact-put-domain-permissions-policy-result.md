---
description: PutDomainPermissionsPolicyResult schema from Amazon CodeArtifact API
layout: schema
name: PutDomainPermissionsPolicyResult
properties_list:
- description: ''
  name: policy
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-put-domain-permissions-policy-result-schema.json
slug: codeartifact-put-domain-permissions-policy-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-domain-permissions-policy-result-schema.json\",\n  \"title\": \"PutDomainPermissionsPolicyResult\",\n  \"description\": \"PutDomainPermissionsPolicyResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicy\"\n        },\n        {\n          \"description\": \" The resource policy that was set after processing the request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-domain-permissions-policy-result-schema.json
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
title: PutDomainPermissionsPolicyResult
---
