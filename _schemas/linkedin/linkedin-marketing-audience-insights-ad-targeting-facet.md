---
description: AdTargetingFacet from LinkedIn API
layout: schema
name: AdTargetingFacet
properties_list:
- description: Name of the targeting facet
  name: facetName
  type: string
- description: URN identifier for the facet
  name: urn
  type: string
- description: Types of entities in this facet
  name: entityTypes
  type: array
- description: Available methods to find entities
  name: availableEntityFinders
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-marketing-audience-insights-ad-targeting-facet-schema.json
slug: linkedin-marketing-audience-insights-ad-targeting-facet
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-ad-targeting-facet-schema.json\",\n  \"title\": \"AdTargetingFacet\",\n  \"description\": \"AdTargetingFacet from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"facetName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the targeting facet\",\n      \"example\": \"jobFunctions\"\n    },\n    \"urn\": {\n      \"type\": \"string\",\n      \"description\": \"URN identifier for the facet\",\n      \"example\": \"urn:li:adTargetingFacet:jobFunctions\"\n    },\n    \"entityTypes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Types of entities in this facet\",\n      \"example\": [\n        \"FUNCTION\"\n      ]\n    },\n    \"availableEntityFinders\": {\n      \"type\"\
  : \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"AD_TARGETING_FACET\",\n          \"TYPEAHEAD\",\n          \"SIMILAR_ENTITIES\"\n        ]\n      },\n      \"description\": \"Available methods to find entities\",\n      \"example\": [\n        \"AD_TARGETING_FACET\"\n      ]\n    }\n  },\n  \"required\": [\n    \"facetName\",\n    \"urn\",\n    \"entityTypes\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-marketing-audience-insights-ad-targeting-facet-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdTargetingFacet
---
