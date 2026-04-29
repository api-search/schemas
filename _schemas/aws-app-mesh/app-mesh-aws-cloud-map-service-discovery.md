---
description: <p>An object that represents the Cloud Map service discovery information for your virtual node.</p> <note> <p>Cloud Map is not available in the eu-south-1 Region.</p> </note>
layout: schema
name: AwsCloudMapServiceDiscovery
properties_list:
- description: ''
  name: attributes
  type: object
- description: ''
  name: ipPreference
  type: object
- description: ''
  name: namespaceName
  type: object
- description: ''
  name: serviceName
  type: object
provider_name: AWS App Mesh
provider_slug: aws-app-mesh
schema_file: json-schema/app-mesh-aws-cloud-map-service-discovery-schema.json
slug: app-mesh-aws-cloud-map-service-discovery
source_filename: app-mesh-aws-cloud-map-service-discovery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCloudMapInstanceAttributes\"\n        },\n        {\n          \"description\": \"A string map that contains attributes with values that you can use to filter instances by any custom attribute that you specified when you registered the instance. Only instances that match all of the specified key/value pairs will be returned.\"\n        }\n      ]\n    },\n    \"ipPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IpPreference\"\n        },\n        {\n          \"description\": \"The preferred IP version that this virtual node uses. Setting the IP preference on the virtual node only overrides the IP preference set for the mesh on this specific node.\"\n        }\n      ]\n    },\n    \"namespaceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCloudMapName\"\
  \n        },\n        {\n          \"description\": \"The name of the Cloud Map namespace to use.\"\n        }\n      ]\n    },\n    \"serviceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCloudMapName\"\n        },\n        {\n          \"description\": \"The name of the Cloud Map service to use.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"namespaceName\",\n    \"serviceName\"\n  ],\n  \"description\": \"<p>An object that represents the Cloud Map service discovery information for your virtual node.</p> <note> <p>Cloud Map is not available in the eu-south-1 Region.</p> </note>\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-aws-cloud-map-service-discovery-schema.json\",\n  \"title\": \"AwsCloudMapServiceDiscovery\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-app-mesh/refs/heads/main/json-schema/app-mesh-aws-cloud-map-service-discovery-schema.json
tags:
- AWS
- Deprecated
- Envoy
- Microservices
- Networking
- Service Mesh
title: AwsCloudMapServiceDiscovery
---
