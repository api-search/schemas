---
description: <p>An object that represents the Cloud Map attribute information for your virtual node.</p> <note> <p>Cloud Map is not available in the eu-south-1 Region.</p> </note>
layout: schema
name: AwsCloudMapInstanceAttribute
properties_list:
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-aws-cloud-map-instance-attribute-schema.json
slug: app-mesh-aws-cloud-map-instance-attribute
source_filename: app-mesh-aws-cloud-map-instance-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCloudMapInstanceAttributeKey\"\n        },\n        {\n          \"description\": \"The name of an Cloud Map service instance attribute key. Any Cloud Map service instance that contains the specified key and value is returned.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCloudMapInstanceAttributeValue\"\n        },\n        {\n          \"description\": \"The value of an Cloud Map service instance attribute key. Any Cloud Map service instance that contains the specified key and value is returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"key\",\n    \"value\"\n  ],\n  \"description\": \"<p>An object that represents the Cloud Map attribute information for your virtual node.</p> <note> <p>Cloud Map is not available in the eu-south-1 Region.</p>\
  \ </note>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-aws-cloud-map-instance-attribute-schema.json\",\n  \"title\": \"AwsCloudMapInstanceAttribute\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-aws-cloud-map-instance-attribute-schema.json
tags:
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: AwsCloudMapInstanceAttribute
---
