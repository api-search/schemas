---
description: DescribeRepositoryResult schema from Amazon CodeArtifact API
layout: schema
name: DescribeRepositoryResult
properties_list:
- description: ''
  name: repository
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-describe-repository-result-schema.json
slug: codeartifact-describe-repository-result
source_filename: codeartifact-describe-repository-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-describe-repository-result-schema.json\",\n  \"title\": \"DescribeRepositoryResult\",\n  \"description\": \"DescribeRepositoryResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"repository\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepositoryDescription\"\n        },\n        {\n          \"description\": \" A <code>RepositoryDescription</code> object that contains the requested repository information. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-describe-repository-result-schema.json
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
title: DescribeRepositoryResult
---
