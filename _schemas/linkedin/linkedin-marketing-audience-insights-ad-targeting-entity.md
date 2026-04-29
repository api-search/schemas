---
description: AdTargetingEntity from LinkedIn API
layout: schema
name: AdTargetingEntity
properties_list:
- description: Display name of the entity
  name: name
  type: string
- description: URN identifier for the entity
  name: urn
  type: string
- description: URN of the parent facet
  name: facetUrn
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-ad-targeting-entity-schema.json
slug: linkedin-marketing-audience-insights-ad-targeting-entity
source_filename: linkedin-marketing-audience-insights-ad-targeting-entity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-ad-targeting-entity-schema.json\",\n  \"title\": \"AdTargetingEntity\",\n  \"description\": \"AdTargetingEntity from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the entity\",\n      \"example\": \"United States\"\n    },\n    \"urn\": {\n      \"type\": \"string\",\n      \"description\": \"URN identifier for the entity\",\n      \"example\": \"urn:li:geo:103644278\"\n    },\n    \"facetUrn\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the parent facet\",\n      \"example\": \"urn:li:adTargetingFacet:locations\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"urn\",\n    \"facetUrn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-ad-targeting-entity-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdTargetingEntity
---
