---
description: AwsCloudMapInstanceAttributes schema from AWS App Mesh
layout: schema
name: AwsCloudMapInstanceAttributes
properties_list: []
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-aws-cloud-map-instance-attributes-schema.json
slug: app-mesh-aws-cloud-map-instance-attributes
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"key\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AwsCloudMapInstanceAttributeKey\"\n          },\n          {\n            \"description\": \"The name of an Cloud Map service instance attribute key. Any Cloud Map service instance that contains the specified key and value is returned.\"\n          }\n        ]\n      },\n      \"value\": {\n        \"allOf\": [\n          {\n            \"$ref\": \"#/components/schemas/AwsCloudMapInstanceAttributeValue\"\n          },\n          {\n            \"description\": \"The value of an Cloud Map service instance attribute key. Any Cloud Map service instance that contains the specified key and value is returned.\"\n          }\n        ]\n      }\n    },\n    \"required\": [\n      \"key\",\n      \"value\"\n    ],\n    \"description\": \"<p>An object that represents the Cloud Map attribute information\
  \ for your virtual node.</p> <note> <p>Cloud Map is not available in the eu-south-1 Region.</p> </note>\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-aws-cloud-map-instance-attributes-schema.json\",\n  \"title\": \"AwsCloudMapInstanceAttributes\",\n  \"description\": \"AwsCloudMapInstanceAttributes schema from AWS App Mesh\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-aws-cloud-map-instance-attributes-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: AwsCloudMapInstanceAttributes
---
