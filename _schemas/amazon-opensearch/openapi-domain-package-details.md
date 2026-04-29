---
description: Information on a package that is associated with a domain.
layout: schema
name: DomainPackageDetails
properties_list:
- description: ''
  name: PackageID
  type: object
- description: ''
  name: PackageName
  type: object
- description: ''
  name: PackageType
  type: object
- description: ''
  name: LastUpdated
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: DomainPackageStatus
  type: object
- description: ''
  name: PackageVersion
  type: object
- description: ''
  name: ReferencePath
  type: object
- description: ''
  name: ErrorDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-domain-package-details-schema.json
slug: openapi-domain-package-details
source_filename: openapi-domain-package-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-package-details-schema.json\",\n  \"title\": \"DomainPackageDetails\",\n  \"description\": \"Information on a package that is associated with a domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageID\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageID\"\n        },\n        {\n          \"description\": \"Internal ID of the package.\"\n        }\n      ]\n    },\n    \"PackageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageName\"\n        },\n        {\n          \"description\": \"User specified name of the package.\"\n        }\n      ]\n    },\n    \"PackageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageType\"\n        },\n        {\n     \
  \     \"description\": \"Currently supports only TXT-DICTIONARY.\"\n        }\n      ]\n    },\n    \"LastUpdated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdated\"\n        },\n        {\n          \"description\": \"Timestamp of the most-recent update to the association status.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"Name of the domain you've associated a package with.\"\n        }\n      ]\n    },\n    \"DomainPackageStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainPackageStatus\"\n        },\n        {\n          \"description\": \"State of the association. Values are ASSOCIATING/ASSOCIATION_FAILED/ACTIVE/DISSOCIATING/DISSOCIATION_FAILED.\"\n        }\n      ]\n    },\n    \"PackageVersion\": {\n      \"$ref\": \"#/components/schemas/PackageVersion\"\
  \n    },\n    \"ReferencePath\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReferencePath\"\n        },\n        {\n          \"description\": \"The relative path on Amazon ES nodes, which can be used as synonym_path when the package is synonym file.\"\n        }\n      ]\n    },\n    \"ErrorDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorDetails\"\n        },\n        {\n          \"description\": \"Additional information if the package is in an error state. Null otherwise.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-package-details-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DomainPackageDetails
---
