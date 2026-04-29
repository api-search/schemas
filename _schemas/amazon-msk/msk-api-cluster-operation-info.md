---
description: <p>Returns information about a cluster operation.</p>
layout: schema
name: ClusterOperationInfo
properties_list:
- description: ''
  name: ClientRequestId
  type: object
- description: ''
  name: ClusterArn
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: ErrorInfo
  type: object
- description: ''
  name: OperationArn
  type: object
- description: ''
  name: OperationState
  type: object
- description: ''
  name: OperationSteps
  type: object
- description: ''
  name: OperationType
  type: object
- description: ''
  name: SourceClusterInfo
  type: object
- description: ''
  name: TargetClusterInfo
  type: object
provider_name: Amazon MSK
provider_slug: amazon-msk
schema_file: json-schema/msk-api-cluster-operation-info-schema.json
slug: msk-api-cluster-operation-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-operation-info-schema.json\",\n  \"title\": \"ClusterOperationInfo\",\n  \"description\": \"\\n            <p>Returns information about a cluster operation.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientRequestId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clientRequestId\"\n          },\n          \"description\": \"\\n            <p>The ID of the API request that triggered this operation.</p>\"\n        }\n      ]\n    },\n    \"ClusterArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"clusterArn\"\n          },\n          \"description\": \"\\\
  n            <p>ARN of the cluster.</p>\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"creationTime\"\n          },\n          \"description\": \"\\n            <p>The time that the operation was created.</p>\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endTime\"\n          },\n          \"description\": \"\\n            <p>The time at which the operation finished.</p>\"\n        }\n      ]\n    },\n    \"ErrorInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"errorInfo\"\n          },\n          \"description\": \"\\n            <p>Describes\
  \ the error if the operation fails.</p>\"\n        }\n      ]\n    },\n    \"OperationArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"operationArn\"\n          },\n          \"description\": \"\\n            <p>ARN of the cluster operation.</p>\"\n        }\n      ]\n    },\n    \"OperationState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"operationState\"\n          },\n          \"description\": \"\\n            <p>State of the cluster operation.</p>\"\n        }\n      ]\n    },\n    \"OperationSteps\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__listOfClusterOperationStep\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"operationSteps\"\n          },\n          \"description\": \"\\n            <p>Steps\
  \ completed during the operation.</p>\"\n        }\n      ]\n    },\n    \"OperationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"operationType\"\n          },\n          \"description\": \"\\n            <p>Type of the cluster operation.</p>\"\n        }\n      ]\n    },\n    \"SourceClusterInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MutableClusterInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"sourceClusterInfo\"\n          },\n          \"description\": \"\\n            <p>Information about cluster attributes before a cluster is updated.</p>\"\n        }\n      ]\n    },\n    \"TargetClusterInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MutableClusterInfo\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"targetClusterInfo\"\n          },\n\
  \          \"description\": \"\\n            <p>Information about cluster attributes after a cluster is updated.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-msk/refs/heads/main/json-schema/msk-api-cluster-operation-info-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: ClusterOperationInfo
---
