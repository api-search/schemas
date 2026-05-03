---
description: A web page. Every web page is implicitly assumed to be declared to be of type WebPage.
layout: schema
name: Schema.org WebPage
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: The name of the web page.
  name: name
  type: string
- description: A description of the web page.
  name: description
  type: string
- description: URL of the web page.
  name: url
  type: string
- description: Date on which the content on this web page was last reviewed for accuracy.
  name: lastReviewed
  type: string
- description: Indicates if this web page element is the main subject of the page.
  name: mainContentOfPage
  type: object
- description: Indicates the main image on the page.
  name: primaryImageOfPage
  type: object
- description: A set of links that can help a user understand and navigate a website hierarchy.
  name: breadcrumb
  type: object
- description: Indicates the primary entity described in some page or other CreativeWork.
  name: mainEntity
  type: object
- description: One of the more significant URLs on the page.
  name: significantLink
  type: object
- description: Indicates sections that are particularly speakable.
  name: speakable
  type: object
- description: One of the domain specialties to which this web page's content applies.
  name: specialty
  type: string
- description: A link related to this web page.
  name: relatedLink
  type: object
- description: People or organizations that have reviewed the content on this web page.
  name: reviewedBy
  type: object
- description: The author of this web page.
  name: author
  type: object
- description: The publisher of this web page.
  name: publisher
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: The date on which the page was most recently modified.
  name: dateModified
  type: string
- description: The language of the content.
  name: inLanguage
  type: string
- description: Indicates the WebSite that this page is part of.
  name: isPartOf
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-web-page-schema.json
slug: schema-org-web-page
source_filename: schema-org-web-page-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/web-page.json\",\n  \"title\": \"Schema.org WebPage\",\n  \"description\": \"A web page. Every web page is implicitly assumed to be declared to be of type WebPage.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"name\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"WebPage\", \"AboutPage\", \"CheckoutPage\", \"CollectionPage\", \"ContactPage\", \"FAQPage\", \"ItemPage\", \"MedicalWebPage\", \"ProfilePage\", \"QAPage\", \"RealEstateListing\", \"SearchResultsPage\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the web page.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description\
  \ of the web page.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the web page.\"\n    },\n    \"lastReviewed\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date on which the content on this web page was last reviewed for accuracy.\"\n    },\n    \"mainContentOfPage\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates if this web page element is the main subject of the page.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"WebPageElement\" },\n        \"cssSelector\": { \"type\": \"string\" }\n      }\n    },\n    \"primaryImageOfPage\": {\n      \"$ref\": \"schema-org-image-object-schema.json\",\n      \"description\": \"Indicates the main image on the page.\"\n    },\n    \"breadcrumb\": {\n      \"$ref\": \"schema-org-breadcrumb-list-schema.json\",\n      \"description\": \"A set of links that can help a user understand and\
  \ navigate a website hierarchy.\"\n    },\n    \"mainEntity\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates the primary entity described in some page or other CreativeWork.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"significantLink\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"One of the more significant URLs on the page.\"\n    },\n    \"speakable\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates sections that are particularly speakable.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"SpeakableSpecification\" },\n        \"cssSelector\": { \"oneOf\": [{ \"type\": \"string\" }, { \"type\": \"array\", \"items\": { \"type\": \"string\" } }] },\n        \"\
  xpath\": { \"oneOf\": [{ \"type\": \"string\" }, { \"type\": \"array\", \"items\": { \"type\": \"string\" } }] }\n      }\n    },\n    \"specialty\": {\n      \"type\": \"string\",\n      \"description\": \"One of the domain specialties to which this web page's content applies.\"\n    },\n    \"relatedLink\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"A link related to this web page.\"\n    },\n    \"reviewedBy\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"People or organizations that have reviewed the content on this web page.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\"\
  \ }\n      ],\n      \"description\": \"The author of this web page.\"\n    },\n    \"publisher\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The publisher of this web page.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date on which the page was most recently modified.\"\n    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the content.\"\n    },\n    \"isPartOf\": {\n      \"$ref\": \"schema-org-web-site-schema.json\",\n      \"description\": \"Indicates the WebSite that this page is part of.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\"\
  : \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-web-page-schema.json
tags:
- Schema.org
- Structured Data
- Linked Data
- JSON-LD
- Vocabulary
- SEO
- Web Standards
- RDF
- Ontology
title: Schema.org WebPage
---
