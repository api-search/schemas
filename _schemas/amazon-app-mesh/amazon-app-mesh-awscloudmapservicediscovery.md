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
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
schema_file: json-schema/amazon-app-mesh-awscloudmapservicediscovery-schema.json
slug: amazon-app-mesh-awscloudmapservicediscovery
source_filename: amazon-app-mesh-awscloudmapservicediscovery-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"AwsCloudMapServiceDiscovery\",\n  \"description\": \"<p>An object that represents the Cloud Map service discovery information for your virtual node.</p> <note> <p>Cloud Map is not available in the eu-south-1 Region.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"attributes\": {},\n    \"ipPreference\": {},\n    \"namespaceName\": {},\n    \"serviceName\": {}\n  },\n  \"required\": [\n    \"namespaceName\",\n    \"serviceName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/json-schema/amazon-app-mesh-awscloudmapservicediscovery-schema.json
tags:
- Microservices
- Networking
- Service Mesh
title: AwsCloudMapServiceDiscovery
---
