---
description: The type of EBS volume, standard, gp2, gp3 or io1. See <a href="http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-ebs" target="_blank">Configuring EBS-based Storage</a>for more information.
layout: schema
name: VolumeType
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-volume-type-schema.json
slug: openapi-volume-type
source_filename: openapi-volume-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-volume-type-schema.json\",\n  \"title\": \"VolumeType\",\n  \"description\": \" The type of EBS volume, standard, gp2, gp3 or io1. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-ebs\\\" target=\\\"_blank\\\">Configuring EBS-based Storage</a>for more information.\",\n  \"type\": \"string\",\n  \"enum\": [\n    \"standard\",\n    \"gp2\",\n    \"io1\",\n    \"gp3\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-volume-type-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: VolumeType
---
