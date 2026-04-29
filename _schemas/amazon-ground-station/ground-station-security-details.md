---
description: Information about endpoints.
layout: schema
name: SecurityDetails
properties_list:
- description: ''
  name: roleArn
  type: object
- description: ''
  name: securityGroupIds
  type: object
- description: ''
  name: subnetIds
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-security-details-schema.json
slug: ground-station-security-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-security-details-schema.json\",\n  \"title\": \"SecurityDetails\",\n  \"description\": \"Information about endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"ARN to a role needed for connecting streams to your instances. \"\n        }\n      ]\n    },\n    \"securityGroupIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecurityGroupIdList\"\n        },\n        {\n          \"description\": \"The security groups to attach to the elastic network interfaces.\"\n        }\n      ]\n    },\n    \"subnetIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SubnetList\"\
  \n        },\n        {\n          \"description\": \"A list of subnets where AWS Ground Station places elastic network interfaces to send streams to your instances.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"roleArn\",\n    \"securityGroupIds\",\n    \"subnetIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-security-details-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: SecurityDetails
---
