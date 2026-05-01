---
description: DeleteDomainPermissionsPolicyResult schema from Amazon CodeArtifact API
layout: schema
name: DeleteDomainPermissionsPolicyResult
properties_list:
- description: ''
  name: policy
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-delete-domain-permissions-policy-result-schema.json
slug: codeartifact-delete-domain-permissions-policy-result
source_filename: codeartifact-delete-domain-permissions-policy-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-domain-permissions-policy-result-schema.json\",\n  \"title\": \"DeleteDomainPermissionsPolicyResult\",\n  \"description\": \"DeleteDomainPermissionsPolicyResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"policy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcePolicy\"\n        },\n        {\n          \"description\": \" Information about the deleted resource policy after processing the request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-domain-permissions-policy-result-schema.json
tags:
- Amazon
- Artifact Repository
- Package Management
- DevOps
- Software Supply Chain
- npm
- Maven
- PyPI
- NuGet
title: DeleteDomainPermissionsPolicyResult
---
