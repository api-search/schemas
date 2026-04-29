---
description: Information about an application that processed requests, users that made requests, or downstream services, resources, and applications that an application used.
layout: schema
name: InsightImpactGraphService
properties_list:
- description: ''
  name: ReferenceId
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Names
  type: object
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Edges
  type: object
provider_name: Amazon X-Ray
provider_slug: amazon-xray
schema_file: json-schema/xray-insight-impact-graph-service-schema.json
slug: xray-insight-impact-graph-service
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReferenceId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NullableInteger\"\n        },\n        {\n          \"description\": \"Identifier for the service. Unique within the service map.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Identifier for the service. Unique within the service map.</p> <ul> <li> <p>Amazon Web Services Resource - The type of an Amazon Web Services resource. For example, AWS::EC2::Instance for an application running on Amazon EC2 or AWS::DynamoDB::Table for an Amazon DynamoDB table that the application used. </p> </li> <li> <p>Amazon Web Services Service - The type of an Amazon Web Services service. For example, AWS::DynamoDB for downstream calls to Amazon DynamoDB that didn't target a specific table. </p> </li> <li> <p>Amazon\
  \ Web Services Service - The type of an Amazon Web Services service. For example, AWS::DynamoDB for downstream calls to Amazon DynamoDB that didn't target a specific table. </p> </li> <li> <p>remote - A downstream service of indeterminate type.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The canonical name of the service.\"\n        }\n      ]\n    },\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceNames\"\n        },\n        {\n          \"description\": \"A list of names for the service, including the canonical name.\"\n        }\n      ]\n    },\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Identifier of the Amazon Web Services account in which the service runs.\"\n\
  \        }\n      ]\n    },\n    \"Edges\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InsightImpactGraphEdgeList\"\n        },\n        {\n          \"description\": \"Connections to downstream services.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Information about an application that processed requests, users that made requests, or downstream services, resources, and applications that an application used. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InsightImpactGraphService\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-impact-graph-service-schema.json\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-xray/refs/heads/main/json-schema/xray-insight-impact-graph-service-schema.json
tags:
- Application Performance
- AWS
- Debugging
- Distributed Tracing
- Monitoring
- Observability
title: InsightImpactGraphService
---
