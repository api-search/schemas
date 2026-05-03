---
description: A NuGet package with its metadata, versions, dependencies, deprecation status, and vulnerability information as represented across the NuGet V3 API.
layout: schema
name: NuGet Package
properties_list:
- description: The unique identifier of the NuGet package.
  name: id
  type: string
- description: The full SemVer 2.0.0 version string of the package. May contain build metadata.
  name: version
  type: string
- description: The display title of the package.
  name: title
  type: string
- description: A description of the package and its functionality.
  name: description
  type: string
- description: A short summary of the package.
  name: summary
  type: string
- description: The author or authors of the package.
  name: authors
  type: object
- description: The owner or owners of the package on the package source.
  name: owners
  type: object
- description: Tags associated with the package for categorization and discovery.
  name: tags
  type: object
- description: The language of the package content.
  name: language
  type: string
- description: The URL to the package icon image.
  name: iconUrl
  type: string
- description: The URL to the package license.
  name: licenseUrl
  type: string
- description: A NuGet license expression compliant with NuGet license expression syntax.
  name: licenseExpression
  type: string
- description: The URL to the project home page.
  name: projectUrl
  type: string
- description: A URL for the rendered HTML view of the package README.
  name: readmeUrl
  type: string
- description: The absolute URL to the registration index for this package.
  name: registration
  type: string
- description: The URL to the .nupkg file for the latest version.
  name: packageContent
  type: string
- description: Whether the package is listed and visible in search results. Assumed true if absent.
  name: listed
  type: boolean
- description: An ISO 8601 timestamp of when the package was published. Set to year 1900 on nuget.org when unlisted.
  name: published
  type: string
- description: A timestamp of when the package was first created on the source.
  name: created
  type: string
- description: Whether the package is verified via ID prefix reservation on nuget.org.
  name: verified
  type: boolean
- description: The total number of downloads across all versions.
  name: totalDownloads
  type: integer
- description: Whether the package requires the user to accept a license before installation.
  name: requireLicenseAcceptance
  type: boolean
- description: The minimum NuGet client version required to use this package.
  name: minClientVersion
  type: string
- description: Whether the package version is a prerelease version.
  name: isPrerelease
  type: boolean
- description: The hash of the package encoded in standard base 64.
  name: packageHash
  type: string
- description: The hashing algorithm used to produce the packageHash. Typically SHA512.
  name: packageHashAlgorithm
  type: string
- description: The size of the .nupkg file in bytes.
  name: packageSize
  type: integer
- description: All available versions of the package.
  name: versions
  type: array
- description: The dependencies of the package grouped by target framework.
  name: dependencyGroups
  type: array
- description: The package types defined by the package author.
  name: packageTypes
  type: array
- description: ''
  name: deprecation
  type: object
- description: Security vulnerabilities associated with this package version.
  name: vulnerabilities
  type: array
provider_name: NuGet
provider_slug: nuget
schema_file: json-schema/nuget-package-schema.json
slug: nuget-package
source_filename: nuget-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://nuget.org/schemas/nuget/package.json\",\n  \"title\": \"NuGet Package\",\n  \"description\": \"A NuGet package with its metadata, versions, dependencies, deprecation status, and vulnerability information as represented across the NuGet V3 API.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"version\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the NuGet package.\",\n      \"minLength\": 1,\n      \"maxLength\": 128,\n      \"pattern\": \"^[a-zA-Z0-9._-]+$\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The full SemVer 2.0.0 version string of the package. May contain build metadata.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The display title of the package.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"\
  description\": \"A description of the package and its functionality.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"A short summary of the package.\"\n    },\n    \"authors\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"The author or authors of the package.\"\n    },\n    \"owners\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"The owner or owners of the package on the package source.\"\n    },\n    \"tags\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Tags associated with the package for categorization and discovery.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The language of the package content.\"\n    },\n    \"iconUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the package icon image.\"\n    },\n    \"licenseUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the package license.\"\n    },\n    \"licenseExpression\": {\n      \"type\": \"string\",\n      \"description\": \"A NuGet license expression compliant with NuGet license expression syntax.\"\n    },\n    \"projectUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the project home page.\"\n    },\n    \"readmeUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URL for the rendered HTML view of the package README.\"\n    },\n    \"registration\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The absolute URL to the registration index for this package.\"\
  \n    },\n    \"packageContent\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the .nupkg file for the latest version.\"\n    },\n    \"listed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the package is listed and visible in search results. Assumed true if absent.\"\n    },\n    \"published\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"An ISO 8601 timestamp of when the package was published. Set to year 1900 on nuget.org when unlisted.\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"A timestamp of when the package was first created on the source.\"\n    },\n    \"verified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the package is verified via ID prefix reservation on nuget.org.\"\n    },\n    \"totalDownloads\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n  \
  \    \"description\": \"The total number of downloads across all versions.\"\n    },\n    \"requireLicenseAcceptance\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the package requires the user to accept a license before installation.\"\n    },\n    \"minClientVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The minimum NuGet client version required to use this package.\"\n    },\n    \"isPrerelease\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the package version is a prerelease version.\"\n    },\n    \"packageHash\": {\n      \"type\": \"string\",\n      \"description\": \"The hash of the package encoded in standard base 64.\"\n    },\n    \"packageHashAlgorithm\": {\n      \"type\": \"string\",\n      \"description\": \"The hashing algorithm used to produce the packageHash. Typically SHA512.\",\n      \"enum\": [\"SHA512\"]\n    },\n    \"packageSize\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\"\
  : \"The size of the .nupkg file in bytes.\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"All available versions of the package.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PackageVersion\"\n      }\n    },\n    \"dependencyGroups\": {\n      \"type\": \"array\",\n      \"description\": \"The dependencies of the package grouped by target framework.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DependencyGroup\"\n      }\n    },\n    \"packageTypes\": {\n      \"type\": \"array\",\n      \"description\": \"The package types defined by the package author.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PackageType\"\n      }\n    },\n    \"deprecation\": {\n      \"$ref\": \"#/$defs/Deprecation\"\n    },\n    \"vulnerabilities\": {\n      \"type\": \"array\",\n      \"description\": \"Security vulnerabilities associated with this package version.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Vulnerability\"\n      }\n    }\n  },\n\
  \  \"$defs\": {\n    \"PackageVersion\": {\n      \"type\": \"object\",\n      \"description\": \"A specific version of a package with its download count and registration leaf URL.\",\n      \"required\": [\"version\", \"downloads\"],\n      \"properties\": {\n        \"@id\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The absolute URL to the registration leaf for this version.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The full SemVer 2.0.0 version string.\"\n        },\n        \"downloads\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of downloads for this specific version.\"\n        }\n      }\n    },\n    \"DependencyGroup\": {\n      \"type\": \"object\",\n      \"description\": \"A group of package dependencies applicable to a specific target framework.\",\n      \"properties\": {\n        \"targetFramework\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The target framework moniker. If absent, the group applies to all frameworks.\"\n        },\n        \"dependencies\": {\n          \"type\": \"array\",\n          \"description\": \"The list of package dependencies in this group.\",\n          \"items\": {\n            \"$ref\": \"#/$defs/PackageDependency\"\n          }\n        }\n      }\n    },\n    \"PackageDependency\": {\n      \"type\": \"object\",\n      \"description\": \"A dependency on another NuGet package.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The package ID of the dependency.\"\n        },\n        \"range\": {\n          \"type\": \"string\",\n          \"description\": \"The allowed version range for the dependency. Defaults to any version if absent.\"\n        },\n        \"registration\": {\n          \"type\": \"string\",\n          \"format\": \"\
  uri\",\n          \"description\": \"The URL to the registration index for this dependency.\"\n        }\n      }\n    },\n    \"PackageType\": {\n      \"type\": \"object\",\n      \"description\": \"A package type defined by the package author, such as Dependency or DotnetTool.\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the package type.\"\n        },\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the package type. Only present if explicitly specified.\"\n        }\n      }\n    },\n    \"Deprecation\": {\n      \"type\": \"object\",\n      \"description\": \"Deprecation information indicating a package should no longer be used.\",\n      \"required\": [\"reasons\"],\n      \"properties\": {\n        \"reasons\": {\n          \"type\": \"array\",\n          \"description\": \"The reasons for deprecation.\",\n        \
  \  \"minItems\": 1,\n          \"items\": {\n            \"type\": \"string\",\n            \"enum\": [\"Legacy\", \"CriticalBugs\", \"Other\"]\n          }\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"Additional details about the deprecation.\"\n        },\n        \"alternatePackage\": {\n          \"$ref\": \"#/$defs/AlternatePackage\"\n        }\n      }\n    },\n    \"AlternatePackage\": {\n      \"type\": \"object\",\n      \"description\": \"A recommended replacement package for a deprecated package.\",\n      \"required\": [\"id\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"The ID of the alternate package.\"\n        },\n        \"range\": {\n          \"type\": \"string\",\n          \"description\": \"The allowed version range, or * if any version is acceptable.\"\n        }\n      }\n    },\n    \"Vulnerability\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"A security vulnerability associated with a package version.\",\n      \"required\": [\"advisoryUrl\", \"severity\"],\n      \"properties\": {\n        \"advisoryUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The URL to the security advisory for this vulnerability.\"\n        },\n        \"severity\": {\n          \"type\": \"string\",\n          \"description\": \"The severity level: 0 = Low, 1 = Moderate, 2 = High, 3 = Critical.\",\n          \"enum\": [\"0\", \"1\", \"2\", \"3\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/json-schema/nuget-package-schema.json
tags:
- Package Management
- .NET
- Packages
- Dependencies
- Software Distribution
- Registry
title: NuGet Package
---
