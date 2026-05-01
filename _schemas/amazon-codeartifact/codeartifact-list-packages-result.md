---
description: ListPackagesResult schema from Amazon CodeArtifact API
layout: schema
name: ListPackagesResult
properties_list:
- description: ''
  name: packages
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-list-packages-result-schema.json
slug: codeartifact-list-packages-result
source_filename: codeartifact-list-packages-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-packages-result-schema.json\",\n  \"title\": \"ListPackagesResult\",\n  \"description\": \"ListPackagesResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packages\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageSummaryList\"\n        },\n        {\n          \"description\": \" The list of returned <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageSummary.html\\\">PackageSummary</a> objects. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \" If there are additional results, this is the token for the next set of results.\
  \ \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-packages-result-schema.json
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
title: ListPackagesResult
---
