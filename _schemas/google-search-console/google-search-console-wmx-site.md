---
description: A Search Console site resource representing a verified property. Properties can be URL-prefix properties or domain properties.
layout: schema
name: WmxSite
properties_list:
- description: 'The URL of the site. For URL-prefix properties, this is the full URL including protocol. For domain properties, this uses the sc-domain: prefix (e.g., sc-domain:example.com).'
  name: siteUrl
  type: string
- description: The user's permission level for this site in Search Console.
  name: permissionLevel
  type: string
provider_name: Google Search Console
provider_slug: google-search-console
schema_file: json-schema/google-search-console-wmx-site-schema.json
slug: google-search-console-wmx-site
source_filename: google-search-console-wmx-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WmxSite\",\n  \"type\": \"object\",\n  \"description\": \"A Search Console site resource representing a verified property. Properties can be URL-prefix properties or domain properties.\",\n  \"properties\": {\n    \"siteUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the site. For URL-prefix properties, this is the full URL including protocol. For domain properties, this uses the sc-domain: prefix (e.g., sc-domain:example.com).\"\n    },\n    \"permissionLevel\": {\n      \"type\": \"string\",\n      \"description\": \"The user's permission level for this site in Search Console.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-search-console/refs/heads/main/json-schema/google-search-console-wmx-site-schema.json
tags:
- Analytics
- Google
- Search
- SEO
- Webmaster Tools
title: WmxSite
---
