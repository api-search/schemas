---
description: DeleteDomainResult schema from Amazon CodeArtifact API
layout: schema
name: DeleteDomainResult
properties_list:
- description: ''
  name: domain
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-delete-domain-result-schema.json
slug: codeartifact-delete-domain-result
source_filename: codeartifact-delete-domain-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-domain-result-schema.json\",\n  \"title\": \"DeleteDomainResult\",\n  \"description\": \"DeleteDomainResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainDescription\"\n        },\n        {\n          \"description\": \" Contains information about the deleted domain after processing the request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-delete-domain-result-schema.json
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
title: DeleteDomainResult
---
