---
description: Details about the origin restrictions set on the package. The package origin restrictions determine how new versions of a package can be added to a specific repository.
layout: schema
name: PackageOriginRestrictions
properties_list:
- description: ''
  name: publish
  type: object
- description: ''
  name: upstream
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-origin-restrictions-schema.json
slug: codeartifact-package-origin-restrictions
source_filename: codeartifact-package-origin-restrictions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-origin-restrictions-schema.json\",\n  \"title\": \"PackageOriginRestrictions\",\n  \"description\": \"Details about the origin restrictions set on the package. The package origin restrictions determine how new versions of a package can be added to a specific repository.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"publish\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowPublish\"\n        },\n        {\n          \"description\": \"The package origin configuration that determines if new versions of the package can be published directly to the repository.\"\n        }\n      ]\n    },\n    \"upstream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AllowUpstream\"\n        },\n        {\n          \"description\"\
  : \"The package origin configuration that determines if new versions of the package can be added to the repository from an external connection or upstream source.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"publish\",\n    \"upstream\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-origin-restrictions-schema.json
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
title: PackageOriginRestrictions
---
