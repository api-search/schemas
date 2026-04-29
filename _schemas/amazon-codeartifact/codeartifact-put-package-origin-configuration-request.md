---
description: PutPackageOriginConfigurationRequest schema from Amazon CodeArtifact API
layout: schema
name: PutPackageOriginConfigurationRequest
properties_list:
- description: ''
  name: restrictions
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-put-package-origin-configuration-request-schema.json
slug: codeartifact-put-package-origin-configuration-request
source_filename: codeartifact-put-package-origin-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-package-origin-configuration-request-schema.json\",\n  \"title\": \"PutPackageOriginConfigurationRequest\",\n  \"description\": \"PutPackageOriginConfigurationRequest schema from Amazon CodeArtifact API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"restrictions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageOriginRestrictions\"\n        },\n        {\n          \"description\": \"<p>A <a href=\\\"https://docs.aws.amazon.com/codeartifact/latest/APIReference/API_PackageOriginRestrictions.html\\\">PackageOriginRestrictions</a> object that contains information about the <code>upstream</code> and <code>publish</code> package origin restrictions. The <code>upstream</code> restriction determines if new package versions can be ingested or retained\
  \ from external connections or upstream repositories. The <code>publish</code> restriction determines if new package versions can be published directly to the repository.</p> <p>You must include both the desired <code>upstream</code> and <code>publish</code> restrictions.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"restrictions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-put-package-origin-configuration-request-schema.json
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
title: PutPackageOriginConfigurationRequest
---
