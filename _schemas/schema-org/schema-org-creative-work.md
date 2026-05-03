---
description: The most generic kind of creative work, including books, movies, photographs, software programs, etc.
layout: schema
name: Schema.org CreativeWork
properties_list:
- description: The Schema.org type.
  name: '@type'
  type: string
- description: The JSON-LD context URL.
  name: '@context'
  type: string
- description: The name of the creative work.
  name: name
  type: string
- description: Headline of the article.
  name: headline
  type: string
- description: A secondary title of the CreativeWork.
  name: alternativeHeadline
  type: string
- description: A description of the creative work.
  name: description
  type: string
- description: The textual content of this CreativeWork.
  name: text
  type: string
- description: An abstract is a short description that summarizes a CreativeWork.
  name: abstract
  type: string
- description: URL of the creative work.
  name: url
  type: string
- description: An image of the creative work.
  name: image
  type: object
- description: The author of this content.
  name: author
  type: object
- description: The creator/author of this CreativeWork.
  name: creator
  type: object
- description: Specifies the Person who edited the CreativeWork.
  name: editor
  type: object
- description: The publisher of the creative work.
  name: publisher
  type: object
- description: A secondary contributor to the CreativeWork.
  name: contributor
  type: object
- description: Date of first broadcast/publication.
  name: datePublished
  type: string
- description: The date on which the CreativeWork was created.
  name: dateCreated
  type: string
- description: The date on which the CreativeWork was most recently modified.
  name: dateModified
  type: string
- description: The year during which the claimed copyright was first asserted.
  name: copyrightYear
  type: integer
- description: The party holding the legal copyright to the CreativeWork.
  name: copyrightHolder
  type: object
- description: A license document that applies to this content.
  name: license
  type: object
- description: The language of the content (IETF BCP 47).
  name: inLanguage
  type: string
- description: Keywords or tags used to describe this content.
  name: keywords
  type: object
- description: Genre of the creative work.
  name: genre
  type: string
- description: The subject matter of the content.
  name: about
  type: object
- description: Indicates an item that this item is part of.
  name: isPartOf
  type: object
- description: Indicates an item that is part of this item.
  name: hasPart
  type: object
- description: The position of an item in a series or sequence of items.
  name: position
  type: object
- description: The version of the CreativeWork.
  name: version
  type: object
- description: A media object that encodes this CreativeWork.
  name: encoding
  type: object
- description: Media type expressed using a MIME format.
  name: encodingFormat
  type: string
- description: The number of interactions for the CreativeWork.
  name: interactionStatistic
  type: object
- description: Comments on this creative work.
  name: comment
  type: object
- description: The number of comments this CreativeWork has received.
  name: commentCount
  type: integer
- description: A review of the item.
  name: review
  type: object
- description: The overall rating.
  name: aggregateRating
  type: object
- description: An offer to provide this item.
  name: offers
  type: object
- description: The human sensory perceptual system or cognitive faculty through which a person may process the content.
  name: accessMode
  type: string
- description: Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility.
  name: accessibilityFeature
  type: object
- description: URL of a reference Web page that unambiguously indicates the item's identity.
  name: sameAs
  type: object
- description: The identifier property represents any kind of identifier.
  name: identifier
  type: string
provider_name: Schema.org
provider_slug: schema-org
schema_file: json-schema/schema-org-creative-work-schema.json
slug: schema-org-creative-work
source_filename: schema-org-creative-work-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.org/schemas/creative-work.json\",\n  \"title\": \"Schema.org CreativeWork\",\n  \"description\": \"The most generic kind of creative work, including books, movies, photographs, software programs, etc.\",\n  \"type\": \"object\",\n  \"required\": [\"@type\"],\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The Schema.org type.\",\n      \"enum\": [\"CreativeWork\", \"Article\", \"Blog\", \"Book\", \"Clip\", \"Comment\", \"Conversation\", \"Course\", \"Dataset\", \"DigitalDocument\", \"Drawing\", \"Episode\", \"Game\", \"Guide\", \"HowTo\", \"LegislationObject\", \"Map\", \"MediaObject\", \"Menu\", \"Message\", \"Movie\", \"MusicComposition\", \"MusicPlaylist\", \"MusicRecording\", \"Painting\", \"Photograph\", \"Play\", \"Poster\", \"PublicationIssue\", \"PublicationVolume\", \"Quotation\", \"Review\", \"Sculpture\", \"Season\", \"ShortStory\"\
  , \"SoftwareApplication\", \"SoftwareSourceCode\", \"TVSeries\", \"Thesis\", \"VisualArtwork\", \"WebContent\", \"WebPage\", \"WebSite\"]\n    },\n    \"@context\": {\n      \"type\": \"string\",\n      \"description\": \"The JSON-LD context URL.\",\n      \"default\": \"https://schema.org\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the creative work.\"\n    },\n    \"headline\": {\n      \"type\": \"string\",\n      \"maxLength\": 110,\n      \"description\": \"Headline of the article.\"\n    },\n    \"alternativeHeadline\": {\n      \"type\": \"string\",\n      \"description\": \"A secondary title of the CreativeWork.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the creative work.\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The textual content of this CreativeWork.\"\n    },\n    \"abstract\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"An abstract is a short description that summarizes a CreativeWork.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the creative work.\"\n    },\n    \"image\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"$ref\": \"schema-org-image-object-schema.json\" }\n      ],\n      \"description\": \"An image of the creative work.\"\n    },\n    \"author\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"$ref\": \"schema-org-person-schema.json\" }, { \"$ref\": \"schema-org-organization-schema.json\" }] } }\n      ],\n      \"description\": \"The author of this content.\"\n    },\n    \"creator\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\"\
  \ }\n      ],\n      \"description\": \"The creator/author of this CreativeWork.\"\n    },\n    \"editor\": {\n      \"$ref\": \"schema-org-person-schema.json\",\n      \"description\": \"Specifies the Person who edited the CreativeWork.\"\n    },\n    \"publisher\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The publisher of the creative work.\"\n    },\n    \"contributor\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"oneOf\": [{ \"$ref\": \"schema-org-person-schema.json\" }, { \"$ref\": \"schema-org-organization-schema.json\" }] } }\n      ],\n      \"description\": \"A secondary contributor to the CreativeWork.\"\n    },\n    \"datePublished\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n\
  \      \"description\": \"Date of first broadcast/publication.\"\n    },\n    \"dateCreated\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date on which the CreativeWork was created.\"\n    },\n    \"dateModified\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"The date on which the CreativeWork was most recently modified.\"\n    },\n    \"copyrightYear\": {\n      \"type\": \"integer\",\n      \"description\": \"The year during which the claimed copyright was first asserted.\"\n    },\n    \"copyrightHolder\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-person-schema.json\" },\n        { \"$ref\": \"schema-org-organization-schema.json\" }\n      ],\n      \"description\": \"The party holding the legal copyright to the CreativeWork.\"\n    },\n    \"license\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"object\", \"properties\": { \"\
  @type\": { \"const\": \"CreativeWork\" }, \"name\": { \"type\": \"string\" }, \"url\": { \"type\": \"string\", \"format\": \"uri\" } } }\n      ],\n      \"description\": \"A license document that applies to this content.\"\n    },\n    \"inLanguage\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the content (IETF BCP 47).\"\n    },\n    \"keywords\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Keywords or tags used to describe this content.\"\n    },\n    \"genre\": {\n      \"type\": \"string\",\n      \"description\": \"Genre of the creative work.\"\n    },\n    \"about\": {\n      \"type\": \"object\",\n      \"description\": \"The subject matter of the content.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    },\n    \"isPartOf\": {\n      \"oneOf\": [\n\
  \        { \"$ref\": \"#\" },\n        { \"type\": \"string\", \"format\": \"uri\" }\n      ],\n      \"description\": \"Indicates an item that this item is part of.\"\n    },\n    \"hasPart\": {\n      \"oneOf\": [\n        { \"$ref\": \"#\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"#\" } }\n      ],\n      \"description\": \"Indicates an item that is part of this item.\"\n    },\n    \"position\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"integer\" }\n      ],\n      \"description\": \"The position of an item in a series or sequence of items.\"\n    },\n    \"version\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"number\" }\n      ],\n      \"description\": \"The version of the CreativeWork.\"\n    },\n    \"encoding\": {\n      \"$ref\": \"schema-org-media-object-schema.json\",\n      \"description\": \"A media object that encodes this CreativeWork.\"\n    },\n    \"encodingFormat\": {\n    \
  \  \"type\": \"string\",\n      \"description\": \"Media type expressed using a MIME format.\"\n    },\n    \"interactionStatistic\": {\n      \"type\": \"object\",\n      \"description\": \"The number of interactions for the CreativeWork.\",\n      \"properties\": {\n        \"@type\": { \"type\": \"string\", \"const\": \"InteractionCounter\" },\n        \"interactionType\": { \"type\": \"string\", \"description\": \"The Action representing the interaction.\" },\n        \"userInteractionCount\": { \"type\": \"integer\", \"description\": \"The number of interactions.\" }\n      }\n    },\n    \"comment\": {\n      \"oneOf\": [\n        { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"Comment\" }, \"text\": { \"type\": \"string\" } } },\n        { \"type\": \"array\", \"items\": { \"type\": \"object\", \"properties\": { \"@type\": { \"const\": \"Comment\" }, \"text\": { \"type\": \"string\" } } } }\n      ],\n      \"description\": \"Comments on this creative work.\"\
  \n    },\n    \"commentCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of comments this CreativeWork has received.\"\n    },\n    \"review\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-review-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-review-schema.json\" } }\n      ],\n      \"description\": \"A review of the item.\"\n    },\n    \"aggregateRating\": {\n      \"$ref\": \"schema-org-aggregate-rating-schema.json\",\n      \"description\": \"The overall rating.\"\n    },\n    \"offers\": {\n      \"oneOf\": [\n        { \"$ref\": \"schema-org-offer-schema.json\" },\n        { \"type\": \"array\", \"items\": { \"$ref\": \"schema-org-offer-schema.json\" } }\n      ],\n      \"description\": \"An offer to provide this item.\"\n    },\n    \"accessMode\": {\n      \"type\": \"string\",\n      \"description\": \"The human sensory perceptual system or cognitive faculty through which a person may process the content.\"\
  \n    },\n    \"accessibilityFeature\": {\n      \"oneOf\": [\n        { \"type\": \"string\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n      ],\n      \"description\": \"Content features of the resource, such as accessible media, alternatives and supported enhancements for accessibility.\"\n    },\n    \"sameAs\": {\n      \"oneOf\": [\n        { \"type\": \"string\", \"format\": \"uri\" },\n        { \"type\": \"array\", \"items\": { \"type\": \"string\", \"format\": \"uri\" } }\n      ],\n      \"description\": \"URL of a reference Web page that unambiguously indicates the item's identity.\"\n    },\n    \"identifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier property represents any kind of identifier.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schema-org/refs/heads/main/json-schema/schema-org-creative-work-schema.json
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
title: Schema.org CreativeWork
---
