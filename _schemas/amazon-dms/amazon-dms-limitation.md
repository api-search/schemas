---
description: <p>Provides information about the limitations of target Amazon Web Services engines.</p> <p>Your source database might include features that the target Amazon Web Services engine doesn't support. Fleet Advisor lists these features as limitations. You should consider these limitations during database migration. For each limitation, Fleet Advisor recommends an action that you can take to address or avoid this limitation.</p>
layout: schema
name: Limitation
properties_list:
- description: ''
  name: DatabaseId
  type: object
- description: ''
  name: EngineName
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Impact
  type: object
- description: ''
  name: Type
  type: object
provider_name: Amazon DMS
provider_slug: amazon-dms
schema_file: json-schema/amazon-dms-limitation-schema.json
slug: amazon-dms-limitation
source_filename: amazon-dms-limitation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-limitation-schema.json\",\n  \"title\": \"Limitation\",\n  \"description\": \"<p>Provides information about the limitations of target Amazon Web Services engines.</p> <p>Your source database might include features that the target Amazon Web Services engine doesn't support. Fleet Advisor lists these features as limitations. You should consider these limitations during database migration. For each limitation, Fleet Advisor recommends an action that you can take to address or avoid this limitation.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DatabaseId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The identifier of the source database.\"\n        }\n      ]\n    },\n    \"EngineName\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the target engine that Fleet Advisor should use in the target engine recommendation. Valid values include <code>\\\"rds-aurora-mysql\\\"</code>, <code>\\\"rds-aurora-postgresql\\\"</code>, <code>\\\"rds-mysql\\\"</code>, <code>\\\"rds-oracle\\\"</code>, <code>\\\"rds-sql-server\\\"</code>, and <code>\\\"rds-postgresql\\\"</code>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the limitation. Describes unsupported database features, migration action items, and other limitations.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"A description of the limitation.\
  \ Provides additional information about the limitation, and includes recommended actions that you can take to address or avoid this limitation.\"\n        }\n      ]\n    },\n    \"Impact\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The impact of the limitation. You can use this parameter to prioritize limitations that you want to address. Valid values include <code>\\\"Blocker\\\"</code>, <code>\\\"High\\\"</code>, <code>\\\"Medium\\\"</code>, and <code>\\\"Low\\\"</code>.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The type of the limitation, such as action required, upgrade required, and limited feature.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-dms/refs/heads/main/json-schema/amazon-dms-limitation-schema.json
tags:
- AWS
- Data Replication
- Database
- Database Migration
- Migration
title: Limitation
---
