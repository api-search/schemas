---
description: The replicated Region information for a directory.
layout: schema
name: RegionDescription
properties_list:
- description: ''
  name: DirectoryId
  type: object
- description: ''
  name: RegionName
  type: object
- description: ''
  name: RegionType
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: VpcSettings
  type: object
- description: ''
  name: DesiredNumberOfDomainControllers
  type: object
- description: ''
  name: LaunchTime
  type: object
- description: ''
  name: StatusLastUpdatedDateTime
  type: object
- description: ''
  name: LastUpdatedDateTime
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-region-description-schema.json
slug: amazon-directory-service-region-description
source_filename: amazon-directory-service-region-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-region-description-schema.json\",\n  \"title\": \"RegionDescription\",\n  \"description\": \"The replicated Region information for a directory.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DirectoryId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryId\"\n        },\n        {\n          \"description\": \"The identifier of the directory.\"\n        }\n      ]\n    },\n    \"RegionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionName\"\n        },\n        {\n          \"description\": \"The name of the Region. For example, <code>us-east-1</code>.\"\n        }\n      ]\n    },\n    \"RegionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RegionType\"\
  \n        },\n        {\n          \"description\": \"Specifies whether the Region is the primary Region or an additional Region.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DirectoryStage\"\n        },\n        {\n          \"description\": \"The status of the replication process for the specified Region.\"\n        }\n      ]\n    },\n    \"VpcSettings\": {\n      \"$ref\": \"#/components/schemas/DirectoryVpcSettings\"\n    },\n    \"DesiredNumberOfDomainControllers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredNumberOfDomainControllers\"\n        },\n        {\n          \"description\": \"The desired number of domain controllers in the specified Region for the specified directory.\"\n        }\n      ]\n    },\n    \"LaunchTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LaunchTime\"\n        },\n        {\n          \"description\"\
  : \"Specifies when the Region replication began.\"\n        }\n      ]\n    },\n    \"StatusLastUpdatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StateLastUpdatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the Region status was last updated.\"\n        }\n      ]\n    },\n    \"LastUpdatedDateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastUpdatedDateTime\"\n        },\n        {\n          \"description\": \"The date and time that the Region description was last updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-region-description-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: RegionDescription
---
