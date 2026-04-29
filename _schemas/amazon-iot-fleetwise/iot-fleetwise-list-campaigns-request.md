---
description: ListCampaignsRequest schema
layout: schema
name: ListCampaignsRequest
properties_list:
- description: ''
  name: nextToken
  type: object
- description: ''
  name: maxResults
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-list-campaigns-request-schema.json
slug: iot-fleetwise-list-campaigns-request
source_filename: iot-fleetwise-list-campaigns-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-campaigns-request-schema.json\",\n  \"title\": \"ListCampaignsRequest\",\n  \"description\": \"ListCampaignsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/nextToken\"\n        },\n        {\n          \"description\": \"<p>A pagination token for the next set of results.</p> <p>If the results of a search are large, only a portion of the results are returned, and a <code>nextToken</code> pagination token is returned in the response. To retrieve the next set of results, reissue the search request and include the returned token. When all results have been returned, the response does not contain a pagination token value. </p>\"\n        }\n      ]\n    },\n    \"maxResults\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/maxResults\"\n        },\n        {\n          \"description\": \" The maximum number of items to return, between 1 and 100, inclusive. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/status\"\n        },\n        {\n          \"description\": \"Optional parameter to filter the results by the status of each created campaign in your account. The status can be one of: <code>CREATING</code>, <code>WAITING_FOR_APPROVAL</code>, <code>RUNNING</code>, or <code>SUSPENDED</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-list-campaigns-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: ListCampaignsRequest
---
