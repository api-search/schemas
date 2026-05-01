---
description: Contains information about the external connection of a repository.
layout: schema
name: RepositoryExternalConnectionInfo
properties_list:
- description: ''
  name: externalConnectionName
  type: object
- description: ''
  name: packageFormat
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon CodeArtifact
provider_slug: amazon-codeartifact
schema_file: json-schema/codeartifact-repository-external-connection-info-schema.json
slug: codeartifact-repository-external-connection-info
source_filename: codeartifact-repository-external-connection-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-repository-external-connection-info-schema.json\",\n  \"title\": \"RepositoryExternalConnectionInfo\",\n  \"description\": \" Contains information about the external connection of a repository. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalConnectionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalConnectionName\"\n        },\n        {\n          \"description\": \" The name of the external connection associated with a repository. \"\n        }\n      ]\n    },\n    \"packageFormat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageFormat\"\n        },\n        {\n          \"description\": \"<p> The package format associated with a repository's external connection. The valid package formats\
  \ are: </p> <ul> <li> <p> <code>npm</code>: A Node Package Manager (npm) package. </p> </li> <li> <p> <code>pypi</code>: A Python Package Index (PyPI) package. </p> </li> <li> <p> <code>maven</code>: A Maven package that contains compiled code in a distributable format, such as a JAR file. </p> </li> <li> <p> <code>nuget</code>: A NuGet package. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalConnectionStatus\"\n        },\n        {\n          \"description\": \" The status of the external connection of a repository. There is one valid value, <code>Available</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeartifact/refs/heads/main/json-schema/codeartifact-repository-external-connection-info-schema.json
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
title: RepositoryExternalConnectionInfo
---
