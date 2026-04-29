---
description: ListRobotApplicationsResponse schema from openapi
layout: schema
name: ListRobotApplicationsResponse
properties_list:
- description: ''
  name: robotApplicationSummaries
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-list-robot-applications-response-schema.json
slug: amazon-robomaker-openapi-list-robot-applications-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-robot-applications-response-schema.json\",\n  \"title\": \"ListRobotApplicationsResponse\",\n  \"description\": \"ListRobotApplicationsResponse schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"robotApplicationSummaries\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotApplicationSummaries\"\n        },\n        {\n          \"description\": \"A list of robot application summaries that meet the criteria of the request.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If the previous paginated request did not return all of the remaining results, the response object's\
  \ <code>nextToken</code> parameter value is set to a token. To retrieve the next set of results, call <code>ListRobotApplications</code> again and assign that token to the request object's <code>nextToken</code> parameter. If there are no remaining results, the previous response object's NextToken parameter is set to null. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-robot-applications-response-schema.json
tags:
- AWS
- Robotics
- Simulation
title: ListRobotApplicationsResponse
---
