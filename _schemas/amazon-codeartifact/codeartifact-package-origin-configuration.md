---
description: Details about the package origin configuration of a package.
layout: schema
name: PackageOriginConfiguration
properties_list:
- description: ''
  name: restrictions
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-package-origin-configuration-schema.json
slug: codeartifact-package-origin-configuration
source_filename: codeartifact-package-origin-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-origin-configuration-schema.json\",\n  \"title\": \"PackageOriginConfiguration\",\n  \"description\": \"Details about the package origin configuration of a package.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"restrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageOriginRestrictions\"\n        },\n        {\n          \"description\": \"A <code>PackageOriginRestrictions</code> object that contains information about the upstream and publish package origin configuration for the package.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-package-origin-configuration-schema.json
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
title: PackageOriginConfiguration
---
