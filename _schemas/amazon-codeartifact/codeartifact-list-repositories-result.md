---
description: ListRepositoriesResult schema from Amazon CodeArtifact API
layout: schema
name: ListRepositoriesResult
properties_list:
- description: ''
  name: repositories
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-list-repositories-result-schema.json
slug: codeartifact-list-repositories-result
source_filename: codeartifact-list-repositories-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-repositories-result-schema.json\",\n  \"title\": \"ListRepositoriesResult\",\n  \"description\": \"ListRepositoriesResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repositories\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositorySummaryList\"\n        },\n        {\n          \"description\": \" The returned list of <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_RepositorySummary.html\\\">RepositorySummary</a> objects. \"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \" If there are additional results, this is the token\
  \ for the next set of results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-list-repositories-result-schema.json
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
title: ListRepositoriesResult
---
