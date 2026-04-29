---
description: EndpointAuthorizations schema from Amazon Redshift
layout: schema
name: EndpointAuthorizations
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-endpoint-authorizations-schema.json
slug: redshift-endpoint-authorizations
source_filename: redshift-endpoint-authorizations-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"object\",\n    \"properties\": {\n      \"Grantor\": {},\n      \"Grantee\": {},\n      \"ClusterIdentifier\": {},\n      \"AuthorizeTime\": {},\n      \"ClusterStatus\": {},\n      \"Status\": {},\n      \"AllowedAllVPCs\": {},\n      \"AllowedVPCs\": {},\n      \"EndpointCount\": {}\n    },\n    \"description\": \"Describes an endpoint authorization for authorizing Redshift-managed VPC endpoint access to a cluster across Amazon Web Services accounts.\"\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-authorizations-schema.json\",\n  \"title\": \"EndpointAuthorizations\",\n  \"description\": \"EndpointAuthorizations schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-endpoint-authorizations-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: EndpointAuthorizations
---
