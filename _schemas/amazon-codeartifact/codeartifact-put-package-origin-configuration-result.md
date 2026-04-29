---
description: PutPackageOriginConfigurationResult schema from Amazon CodeArtifact API
layout: schema
name: PutPackageOriginConfigurationResult
properties_list:
- description: ''
  name: originConfiguration
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-put-package-origin-configuration-result-schema.json
slug: codeartifact-put-package-origin-configuration-result
source_filename: codeartifact-put-package-origin-configuration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-package-origin-configuration-result-schema.json\",\n  \"title\": \"PutPackageOriginConfigurationResult\",\n  \"description\": \"PutPackageOriginConfigurationResult schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"originConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageOriginConfiguration\"\n        },\n        {\n          \"description\": \"A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageOriginConfiguration.html\\\">PackageOriginConfiguration</a> object that describes the origin configuration set for the package. It contains a <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageOriginRestrictions.html\\\">PackageOriginRestrictions</a>\
  \ object that describes how new versions of the package can be introduced to the repository.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-package-origin-configuration-result-schema.json
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
title: PutPackageOriginConfigurationResult
---
