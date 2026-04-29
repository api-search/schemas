---
description: The HTTP package configuration properties for the requested VOD source.
layout: schema
name: HttpPackageConfiguration
properties_list:
- description: ''
  name: Path
  type: object
- description: ''
  name: SourceGroup
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-http-package-configuration-schema.json
slug: mediatailor-api-http-package-configuration
source_filename: mediatailor-api-http-package-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-http-package-configuration-schema.json\",\n  \"title\": \"HttpPackageConfiguration\",\n  \"description\": \"The HTTP package configuration properties for the requested VOD source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Path\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The relative path to the URL for this VOD source. This is combined with <code>SourceLocation::HttpConfiguration::BaseUrl</code> to form a valid URL.\"\n        }\n      ]\n    },\n    \"SourceGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The name of the source group. This has to match one of the <code>Channel::Outputs::SourceGroup</code>.\"\
  \n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Type\"\n        },\n        {\n          \"description\": \"The streaming protocol for this package configuration. Supported values are <code>HLS</code> and <code>DASH</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Path\",\n    \"SourceGroup\",\n    \"Type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-http-package-configuration-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HttpPackageConfiguration
---
