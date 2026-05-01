---
description: Contains directory limit information for a Region.
layout: schema
name: DirectoryLimits
properties_list:
- description: ''
  name: CloudOnlyDirectoriesLimit
  type: object
- description: ''
  name: CloudOnlyDirectoriesCurrentCount
  type: object
- description: ''
  name: CloudOnlyDirectoriesLimitReached
  type: object
- description: ''
  name: CloudOnlyMicrosoftADLimit
  type: object
- description: ''
  name: CloudOnlyMicrosoftADCurrentCount
  type: object
- description: ''
  name: CloudOnlyMicrosoftADLimitReached
  type: object
- description: ''
  name: ConnectedDirectoriesLimit
  type: object
- description: ''
  name: ConnectedDirectoriesCurrentCount
  type: object
- description: ''
  name: ConnectedDirectoriesLimitReached
  type: object
provider_name: Amazon Directory Service
provider_slug: amazon-directory-service
schema_file: json-schema/amazon-directory-service-directory-limits-schema.json
slug: amazon-directory-service-directory-limits
source_filename: amazon-directory-service-directory-limits-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-limits-schema.json\",\n  \"title\": \"DirectoryLimits\",\n  \"description\": \"Contains directory limit information for a Region.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CloudOnlyDirectoriesLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of cloud directories allowed in the Region.\"\n        }\n      ]\n    },\n    \"CloudOnlyDirectoriesCurrentCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The current number of cloud directories in the Region.\"\n        }\n      ]\n    },\n    \"CloudOnlyDirectoriesLimitReached\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/CloudOnlyDirectoriesLimitReached\"\n        },\n        {\n          \"description\": \"Indicates if the cloud directory limit has been reached.\"\n        }\n      ]\n    },\n    \"CloudOnlyMicrosoftADLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of Managed Microsoft AD directories allowed in the region.\"\n        }\n      ]\n    },\n    \"CloudOnlyMicrosoftADCurrentCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The current number of Managed Microsoft AD directories in the region.\"\n        }\n      ]\n    },\n    \"CloudOnlyMicrosoftADLimitReached\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudOnlyDirectoriesLimitReached\"\n        },\n        {\n          \"description\"\
  : \"Indicates if the Managed Microsoft AD directory limit has been reached.\"\n        }\n      ]\n    },\n    \"ConnectedDirectoriesLimit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The maximum number of connected directories allowed in the Region.\"\n        }\n      ]\n    },\n    \"ConnectedDirectoriesCurrentCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Limit\"\n        },\n        {\n          \"description\": \"The current number of connected directories in the Region.\"\n        }\n      ]\n    },\n    \"ConnectedDirectoriesLimitReached\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConnectedDirectoriesLimitReached\"\n        },\n        {\n          \"description\": \"Indicates if the connected directory limit has been reached.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-directory-service/refs/heads/main/json-schema/amazon-directory-service-directory-limits-schema.json
tags:
- Active Directory
- Authentication
- Directory Services
- Identity Management
title: DirectoryLimits
---
