---
description: DomainName schema from Amazon CodeArtifact API
layout: schema
name: DomainName
properties_list: []
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-domain-name-schema.json
slug: codeartifact-domain-name
source_filename: codeartifact-domain-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-name-schema.json\",\n  \"title\": \"DomainName\",\n  \"description\": \"DomainName schema from Amazon CodeArtifact API\",\n  \"type\": \"string\",\n  \"pattern\": \"[a-z][a-z0-9\\\\-]{0,48}[a-z0-9]\",\n  \"minLength\": 2,\n  \"maxLength\": 50\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-domain-name-schema.json
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
title: DomainName
---
