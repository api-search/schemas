---
description: StatementId schema from Amazon Redshift
layout: schema
name: StatementId
properties_list: []
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-data-statement-id-schema.json
slug: redshift-data-statement-id
source_json: "{\n  \"type\": \"string\",\n  \"pattern\": \"^[a-z0-9]{8}(-[a-z0-9]{4}){3}-[a-z0-9]{12}(:\\\\d+)?$\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-statement-id-schema.json\",\n  \"title\": \"StatementId\",\n  \"description\": \"StatementId schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-data-statement-id-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: StatementId
---
