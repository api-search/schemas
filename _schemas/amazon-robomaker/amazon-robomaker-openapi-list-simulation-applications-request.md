---
description: ListSimulationApplicationsRequest schema from openapi
layout: schema
name: ListSimulationApplicationsRequest
properties_list:
- description: ''
  name: versionQualifier
  type: object
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: filters
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-list-simulation-applications-request-schema.json
slug: amazon-robomaker-openapi-list-simulation-applications-request
source_filename: amazon-robomaker-openapi-list-simulation-applications-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-simulation-applications-request-schema.json\",\n  \"title\": \"ListSimulationApplicationsRequest\",\n  \"description\": \"ListSimulationApplicationsRequest schema from openapi\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"versionQualifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VersionQualifier\"\n        },\n        {\n          \"description\": \"The version qualifier of the simulation application.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"If the previous paginated request did not return all of the remaining results, the response object's <code>nextToken</code> parameter\
  \ value is set to a token. To retrieve the next set of results, call <code>ListSimulationApplications</code> again and assign that token to the request object's <code>nextToken</code> parameter. If there are no remaining results, the previous response object's NextToken parameter is set to null. \"\n        }\n      ]\n    },\n    \"maxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"When this parameter is used, <code>ListSimulationApplications</code> only returns <code>maxResults</code> results in a single page along with a <code>nextToken</code> response element. The remaining results of the initial request can be seen by sending another <code>ListSimulationApplications</code> request with the returned <code>nextToken</code> value. This value can be between 1 and 100. If this parameter is not used, then <code>ListSimulationApplications</code> returns up to 100 results and a <code>nextToken</code>\
  \ value if applicable. \"\n        }\n      ]\n    },\n    \"filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Filters\"\n        },\n        {\n          \"description\": \"<p>Optional list of filters to limit results.</p> <p>The filter name <code>name</code> is supported. When filtering, you must use the complete value of the filtered item. You can use up to three filters.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-list-simulation-applications-request-schema.json
tags:
- Robotics
- Simulation
title: ListSimulationApplicationsRequest
---
