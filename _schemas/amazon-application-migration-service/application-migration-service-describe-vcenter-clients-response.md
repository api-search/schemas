---
description: Response with list of vCenter clients
layout: schema
name: DescribeVcenterClientsResponse
properties_list:
- description: List of vCenter clients
  name: items
  type: array
- description: Pagination token
  name: nextToken
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-describe-vcenter-clients-response-schema.json
slug: application-migration-service-describe-vcenter-clients-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-describe-vcenter-clients-response-schema.json\",\n  \"title\": \"DescribeVcenterClientsResponse\",\n  \"description\": \"Response with list of vCenter clients\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of vCenter clients\"\n    },\n    \"nextToken\": {\n      \"type\": \"string\",\n      \"description\": \"Pagination token\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-describe-vcenter-clients-response-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: DescribeVcenterClientsResponse
---
