---
description: StartSimulationInput schema from Amazon SimSpace Weaver API
layout: schema
name: StartSimulationInput
properties_list:
- description: ''
  name: ClientToken
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: MaximumDuration
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SchemaS3Location
  type: object
- description: ''
  name: SnapshotS3Location
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-start-simulation-input-schema.json
slug: amazon-simspace-weaver-start-simulation-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-simulation-input-schema.json\",\n  \"title\": \"StartSimulationInput\",\n  \"description\": \"StartSimulationInput schema from Amazon SimSpace Weaver API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClientToken\"\n        },\n        {\n          \"description\": \"A value that you provide to ensure that repeated calls to this API operation using the same parameters complete only once. A <code>ClientToken</code> is also known as an <i>idempotency token</i>. A <code>ClientToken</code> expires after 24 hours.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Description\"\n        },\n    \
  \    {\n          \"description\": \"The description of the simulation.\"\n        }\n      ]\n    },\n    \"MaximumDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeToLiveString\"\n        },\n        {\n          \"description\": \"The maximum running time of the simulation, specified as a number of minutes (m or M), hours (h or H), or days (d or D). The simulation stops when it reaches this limit. The maximum value is <code>14D</code>, or its equivalent in the other units. The default value is <code>14D</code>. A value equivalent to <code>0</code> makes the simulation immediately transition to <code>Stopping</code> as soon as it reaches <code>Started</code>.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the simulation.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role that the simulation assumes to perform actions. For more information about ARNs, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">Amazon Resource Names (ARNs)</a> in the <i>Amazon Web Services General Reference</i>. For more information about IAM roles, see <a href=\\\"https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html\\\">IAM roles</a> in the <i>Identity and Access Management User Guide</i>.\"\n        }\n      ]\n    },\n    \"SchemaS3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"<p>The location of the simulation schema in Amazon Simple Storage Service (Amazon S3). For more information about Amazon S3, see the\
  \ <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html\\\"> <i>Amazon Simple Storage Service User Guide</i> </a>.</p> <p>Provide a <code>SchemaS3Location</code> to start your simulation from a schema.</p> <p>If you provide a <code>SchemaS3Location</code> then you can't provide a <code>SnapshotS3Location</code>.</p>\"\n        }\n      ]\n    },\n    \"SnapshotS3Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"<p>The location of the snapshot .zip file in Amazon Simple Storage Service (Amazon S3). For more information about Amazon S3, see the <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/Welcome.html\\\"> <i>Amazon Simple Storage Service User Guide</i> </a>.</p> <p>Provide a <code>SnapshotS3Location</code> to start your simulation from a snapshot.</p> <p>The Amazon S3 bucket must be in the same Amazon Web Services Region as the simulation.</p>\
  \ <p>If you provide a <code>SnapshotS3Location</code> then you can't provide a <code>SchemaS3Location</code>.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagMap\"\n        },\n        {\n          \"description\": \"A list of tags for the simulation. For more information about tags, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\">Tagging Amazon Web Services resources</a> in the <i>Amazon Web Services General Reference</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-start-simulation-input-schema.json
tags:
- AWS
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: StartSimulationInput
---
