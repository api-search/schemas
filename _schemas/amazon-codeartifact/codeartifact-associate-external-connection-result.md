---
description: AssociateExternalConnectionResult schema from Amazon CodeArtifact API
layout: schema
name: AssociateExternalConnectionResult
properties_list:
- description: ''
  name: repository
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-associate-external-connection-result-schema.json
slug: codeartifact-associate-external-connection-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-associate-external-connection-result-schema.json\",\n  \"title\": \"AssociateExternalConnectionResult\",\n  \"description\": \"AssociateExternalConnectionResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryDescription\"\n        },\n        {\n          \"description\": \" Information about the connected repository after processing the request. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-associate-external-connection-result-schema.json
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
title: AssociateExternalConnectionResult
---
