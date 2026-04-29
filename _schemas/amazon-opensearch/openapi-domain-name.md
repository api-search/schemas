---
description: 'The name of an Elasticsearch domain. Domain names are unique across the domains owned by an account within an AWS region. Domain names start with a letter or number and can contain the following characters: a-z (lowercase), 0-9, and - (hyphen).'
layout: schema
name: DomainName
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-domain-name-schema.json
slug: openapi-domain-name
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-name-schema.json\",\n  \"title\": \"DomainName\",\n  \"description\": \"The name of an Elasticsearch domain. Domain names are unique across the domains owned by an account within an AWS region. Domain names start with a letter or number and can contain the following characters: a-z (lowercase), 0-9, and - (hyphen).\",\n  \"type\": \"string\",\n  \"pattern\": \"[a-z][a-z0-9\\\\-]+\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-name-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DomainName
---
