---
description: Schema for a Dart/Flutter package as returned by the Pub.dev API, including metadata, versions, and pubspec information.
layout: schema
name: Pub.dev Package
properties_list:
- description: The package name
  name: name
  type: string
- description: ''
  name: latest
  type: object
- description: All published versions of the package
  name: versions
  type: array
provider_name: Google Flutter
provider_slug: google-flutter
schema_file: json-schema/google-flutter-pub-package-schema.json
slug: google-flutter-pub-package
source_filename: google-flutter-pub-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://pub.dev/schemas/package.json\",\n  \"title\": \"Pub.dev Package\",\n  \"description\": \"Schema for a Dart/Flutter package as returned by the Pub.dev API, including metadata, versions, and pubspec information.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The package name\"\n    },\n    \"latest\": {\n      \"$ref\": \"#/$defs/PackageVersion\"\n    },\n    \"versions\": {\n      \"type\": \"array\",\n      \"description\": \"All published versions of the package\",\n      \"items\": {\n        \"$ref\": \"#/$defs/PackageVersion\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"PackageVersion\": {\n      \"type\": \"object\",\n      \"description\": \"A specific version of a package\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Semantic version string\"\n        },\n        \"pubspec\": {\n          \"$ref\": \"#/$defs/Pubspec\"\n        },\n        \"archive_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL to the version archive\"\n        },\n        \"published\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"When this version was published\"\n        }\n      }\n    },\n    \"Pubspec\": {\n      \"type\": \"object\",\n      \"description\": \"The pubspec.yaml contents for a package version\",\n      \"required\": [\"name\", \"version\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"version\": {\n          \"type\": \"string\"\n        },\n        \"description\": {\n          \"type\": \"string\"\n        },\n        \"homepage\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"repository\":\
  \ {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"environment\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"sdk\": {\n              \"type\": \"string\",\n              \"description\": \"Dart SDK version constraint\"\n            },\n            \"flutter\": {\n              \"type\": \"string\",\n              \"description\": \"Flutter SDK version constraint\"\n            }\n          }\n        },\n        \"dependencies\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Package dependencies\"\n        },\n        \"dev_dependencies\": {\n          \"type\": \"object\",\n          \"additionalProperties\": true,\n          \"description\": \"Development-only dependencies\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-flutter/refs/heads/main/json-schema/google-flutter-pub-package-schema.json
tags:
- Cross-Platform
- Dart
- Google
- Mobile Development
- Open Source
- UI Framework
title: Pub.dev Package
---
