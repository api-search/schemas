---
description: The Amazon Resource Name (ARN) of the site.
layout: schema
name: SiteArn
properties_list: []
provider_name: Amazon Outposts
provider_slug: amazon-outposts
schema_file: json-schema/openapi-site-arn-schema.json
slug: openapi-site-arn
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-site-arn-schema.json\",\n  \"title\": \"SiteArn\",\n  \"description\": \"The Amazon Resource Name (ARN) of the site.\",\n  \"type\": \"string\",\n  \"pattern\": \"^arn:aws([a-z-]+)?:outposts:[a-z\\\\d-]+:\\\\d{12}:site/(os-[a-f0-9]{17})$\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-outposts/refs/heads/main/json-schema/openapi-site-arn-schema.json
tags:
- AWS
- Edge Computing
- Hybrid Cloud
- Infrastructure
- On-Premises
title: SiteArn
---
