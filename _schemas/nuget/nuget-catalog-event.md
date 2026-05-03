---
description: A catalog event (leaf) in the NuGet Catalog API representing either a package details snapshot or a package deletion record. The catalog records the full history of all package operations on nuget.org.
layout: schema
name: NuGet Catalog Event
properties_list:
- description: The type(s) of the catalog item. Includes either PackageDetails or PackageDelete, optionally with catalog:Permalink.
  name: '@type'
  type: object
- description: A unique identifier for the commit that produced this catalog item.
  name: catalog:commitId
  type: string
- description: The ISO 8601 timestamp when this item was committed to the catalog.
  name: catalog:commitTimeStamp
  type: string
- description: The package ID of the catalog item.
  name: id
  type: string
- description: The package version string. For PackageDetails, this is normalized. For PackageDelete, this is the original .nuspec version.
  name: version
  type: string
- description: For PackageDetails, when the package was last listed. For PackageDelete, when the package was deleted.
  name: published
  type: string
- description: The original cased package ID. Present only in PackageDelete items.
  name: originalId
  type: string
- description: When the package was first created. Present only in PackageDetails items.
  name: created
  type: string
- description: The package authors. Present only in PackageDetails items.
  name: authors
  type: string
- description: The package description. Present only in PackageDetails items.
  name: description
  type: string
- description: Whether the version is a prerelease. Present only in PackageDetails items.
  name: isPrerelease
  type: boolean
- description: Whether the package is listed. Present only in PackageDetails items.
  name: listed
  type: boolean
- description: Base 64 encoded hash of the .nupkg file. Present only in PackageDetails items.
  name: packageHash
  type: string
- description: The hash algorithm used, typically SHA512. Present only in PackageDetails items.
  name: packageHashAlgorithm
  type: string
- description: Size of the .nupkg file in bytes. Present only in PackageDetails items.
  name: packageSize
  type: integer
- description: The version string as originally found in the .nuspec. Present only in PackageDetails items.
  name: verbatimVersion
  type: string
provider_name: NuGet
provider_slug: nuget
schema_file: json-schema/nuget-catalog-event-schema.json
slug: nuget-catalog-event
source_filename: nuget-catalog-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://nuget.org/schemas/nuget/catalog-event.json\",\n  \"title\": \"NuGet Catalog Event\",\n  \"description\": \"A catalog event (leaf) in the NuGet Catalog API representing either a package details snapshot or a package deletion record. The catalog records the full history of all package operations on nuget.org.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"catalog:commitId\", \"catalog:commitTimeStamp\", \"id\", \"published\", \"version\"],\n  \"properties\": {\n    \"@type\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"The type(s) of the catalog item. Includes either PackageDetails or PackageDelete, optionally with catalog:Permalink.\"\n    },\n    \"catalog:commitId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the commit\
  \ that produced this catalog item.\"\n    },\n    \"catalog:commitTimeStamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when this item was committed to the catalog.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The package ID of the catalog item.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The package version string. For PackageDetails, this is normalized. For PackageDelete, this is the original .nuspec version.\"\n    },\n    \"published\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"For PackageDetails, when the package was last listed. For PackageDelete, when the package was deleted.\"\n    },\n    \"originalId\": {\n      \"type\": \"string\",\n      \"description\": \"The original cased package ID. Present only in PackageDelete items.\"\n    },\n    \"created\": {\n      \"type\": \"string\"\
  ,\n      \"format\": \"date-time\",\n      \"description\": \"When the package was first created. Present only in PackageDetails items.\"\n    },\n    \"authors\": {\n      \"type\": \"string\",\n      \"description\": \"The package authors. Present only in PackageDetails items.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The package description. Present only in PackageDetails items.\"\n    },\n    \"isPrerelease\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the version is a prerelease. Present only in PackageDetails items.\"\n    },\n    \"listed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the package is listed. Present only in PackageDetails items.\"\n    },\n    \"packageHash\": {\n      \"type\": \"string\",\n      \"description\": \"Base 64 encoded hash of the .nupkg file. Present only in PackageDetails items.\"\n    },\n    \"packageHashAlgorithm\": {\n      \"type\": \"string\",\n      \"\
  description\": \"The hash algorithm used, typically SHA512. Present only in PackageDetails items.\"\n    },\n    \"packageSize\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Size of the .nupkg file in bytes. Present only in PackageDetails items.\"\n    },\n    \"verbatimVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version string as originally found in the .nuspec. Present only in PackageDetails items.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/json-schema/nuget-catalog-event-schema.json
tags:
- Package Management
- .NET
- Packages
- Dependencies
- Software Distribution
- Registry
title: NuGet Catalog Event
---
