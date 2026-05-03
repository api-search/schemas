---
description: An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types.
layout: schema
name: Schema.org Article
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: ''
  name: '@context'
  type: string
- description: Headline of the article.
  name: headline
  type: string
- description: A secondary title of the article.
  name: alternativeHeadline
  type: string
- description: The name of the article.
  name: name
  type: string
- description: A short description of the article.
  name: description
  type: string
- description: The actual body of the article.
  name: articleBody
  type: string
- description: Articles may belong to one or more sections in a magazine or newspaper.
  name: articleSection
  type: string
- description: The number of words in the text of the article.
  name: wordCount
  type: integer
- description: The page on which the work starts.
  name: pageStart
  type: string
- description: The page on which the work ends.
  name: pageEnd
  type: string
- description: Any description of pages that is not separated into pageStart and pageEnd.
  name: pagination
  type: string
- description: URL of the article.
  name: url
  type: string
- description: An image for the article.
  name: image
  type: object
- description: The author of this article.
  name: author
  type: object
- description: The publisher of this article.
  name: publisher
  type: object
- description: Date of first publication.
  name: datePublished
  type: string
- description: The date on which the article was created.
  name: dateCreated
  type: string
- description: The date on which the article was most recently modified.
  name: dateModified
  type: string
- description: Keywords or tags used to describe this content.
  name: keywords
  type: object
- description: The language of the content.
  name: inLanguage
  type: string
- description: Indicates an item or CreativeWork that this item is part of.
  name: isPartOf
  type: object
- description: Indicates a page for which this thing is the main entity being described.
  name: mainEntityOfPage
  type: object
- description: Indicates sections of a Web page that are particularly speakable.
  name: speakable
  type: object
- description: For an Article, typically a NewsArticle, the backstory property provides a textual summary of how and why this article was created.
  name: backstory
  type: string
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-article-schema.json
slug: schema-org-article
source_filename: schema-org-article-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/article.json\",\n  \"title\": \"Schema.org Article\",\n  \"description\": \"An article, such as a news article or piece of investigative report. Newspapers and magazines have articles of many different types.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\", \"headline\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"Article\", \"AdvertiserContentArticle\", \"NewsArticle\", \"Report\", \"SatiricalArticle\", \"ScholarlyArticle\", \"SocialMediaPosting\", \"TechArticle\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"default\": \"https://schema.org\"\n    },\n    \"headline\": {\n      \"type\": \"string\",\n      \"maxLength\": 110,\n      \"description\": \"Headline of the article.\"\n    },\n    \"alternativeHeadline\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"A secondary title of the article.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the article.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A short description of the article.\"\n    },\n    \"articleBody\": {\n      \"type\": \"string\",\n      \"description\": \"The actual body of the article.\"\n    },\n    \"articleSection\": {\n      \"type\": \"string\",\n      \"description\": \"Articles may belong to one or more sections in a magazine or newspaper.\"\n    },\n    \"wordCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of words in the text of the article.\"\n    },\n    \"pageStart\": {\n      \"type\": \"string\",\n      \"description\": \"The page on which the work starts.\"\n    },\n    \"pageEnd\": {\n      \"type\": \"string\",\n      \"description\": \"The page on which the work ends.\"\n    },\n    \"pagination\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Any description of pages that is not separated into pageStart and pageEnd.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the article.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"type\": \"string\", \"format\": \"uri\" }, { \"$ref\": \"schema-org-image-object-schema.json\" }] } }\n      ],\n      \"description\": \"An image for the article.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"$ref\": \"schema-org-person-schema.json\" }, { \"$ref\": \"schema-org-organization-schema.json\" }] } }\n      ],\n      \"description\"\
  : \"The author of this article.\"\n    },\n    \"publisher\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The publisher of this article.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date of first publication.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date on which the article was created.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date on which the article was most recently modified.\"\n    },\n    \"keywords\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Keywords or tags used to describe this content.\"\n\
  \    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the content.\"\n    },\n    \"isPartOf\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"object\", \"properties\": { \"@type\": { \"type\": \"string\" }, \"name\": { \"type\": \"string\" } } }\n      ],\n      \"description\": \"Indicates an item or CreativeWork that this item is part of.\"\n    },\n    \"mainEntityOfPage\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-web-page-schema.json\" }\n      ],\n      \"description\": \"Indicates a page for which this thing is the main entity being described.\"\n    },\n    \"speakable\": {\n      \"type\": \"object\",\n      \"description\": \"Indicates sections of a Web page that are particularly speakable.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"SpeakableSpecification\" },\n  \
  \      \"cssSelector\": { \"oneOf\": [{ \"type\": \"string\" }, { \"type\": \"array\", \"items\": { \"type\": \"string\" } }] },\n        \"xpath\": { \"oneOf\": [{ \"type\": \"string\" }, { \"type\": \"array\", \"items\": { \"type\": \"string\" } }] }\n      }\n    },\n    \"backstory\": {\n      \"type\": \"string\",\n      \"description\": \"For an Article, typically a NewsArticle, the backstory property provides a textual summary of how and why this article was created.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-article-schema.json
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
title: Schema.org Article
---
