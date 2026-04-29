---
description: Schema for a Bloomberg news article delivered through the Bloomberg News API or BLPAPI //blp/mktdata and //blp/refdata news services, representing breaking news, analysis, and multimedia content covering global markets and business.
layout: schema
name: Bloomberg News Article
properties_list:
- description: Unique Bloomberg identifier for the news story
  name: storyId
  type: string
- description: Primary headline of the news article
  name: headline
  type: string
- description: Secondary headline or deck providing additional context
  name: subHeadline
  type:
  - string
  - 'null'
- description: Brief summary or abstract of the article content
  name: summary
  type: string
- description: Full text body of the news article
  name: body
  type: string
- description: ISO 8601 timestamp when the article was first published
  name: publishedAt
  type: string
- description: ISO 8601 timestamp when the article was last updated
  name: updatedAt
  type:
  - string
  - 'null'
- description: Canonical URL of the article on Bloomberg.com
  name: url
  type: string
- description: List of authors who contributed to the article
  name: authors
  type: array
- description: Originating news source or wire service
  name: source
  type: string
- description: ISO 639-1 language code of the article
  name: language
  type: string
- description: Total word count of the article body
  name: wordCount
  type: integer
- description: Classification of the article type
  name: articleType
  type: string
- description: News urgency classification reflecting the BLPAPI NEWS_STORY_URGENCY field
  name: urgency
  type: string
- description: Bloomberg topic codes and categories associated with the article
  name: topics
  type: array
- description: Securities mentioned in or related to the article, referenced by Bloomberg identifiers
  name: securities
  type: array
- description: Geographic regions relevant to the article
  name: regions
  type: array
- description: Industry sectors relevant to the article content
  name: sectors
  type: array
- description: Free-form tags or keywords associated with the article
  name: tags
  type: array
- description: Associated multimedia content such as images, videos, or charts
  name: media
  type: array
- description: References to related Bloomberg news stories
  name: relatedStories
  type: array
- description: Copyright notice for the article content
  name: copyright
  type: string
provider_name: Bloomberg News
provider_slug: bloomberg-news
schema_file: json-schema/bloomberg-news-article-schema.json
slug: bloomberg-news-article
source_filename: bloomberg-news-article-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://bloomberg.com/schemas/bloomberg-news/article.json\",\n  \"title\": \"Bloomberg News Article\",\n  \"description\": \"Schema for a Bloomberg news article delivered through the Bloomberg News API or BLPAPI //blp/mktdata and //blp/refdata news services, representing breaking news, analysis, and multimedia content covering global markets and business.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"storyId\",\n    \"headline\",\n    \"publishedAt\"\n  ],\n  \"properties\": {\n    \"storyId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Bloomberg identifier for the news story\"\n    },\n    \"headline\": {\n      \"type\": \"string\",\n      \"description\": \"Primary headline of the news article\",\n      \"maxLength\": 500\n    },\n    \"subHeadline\": {\n      \"type\": [\"string\", \"null\"],\n      \"description\": \"Secondary headline or deck providing additional\
  \ context\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Brief summary or abstract of the article content\"\n    },\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Full text body of the news article\"\n    },\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the article was first published\"\n    },\n    \"updatedAt\": {\n      \"type\": [\"string\", \"null\"],\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the article was last updated\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Canonical URL of the article on Bloomberg.com\"\n    },\n    \"authors\": {\n      \"type\": \"array\",\n      \"description\": \"List of authors who contributed to the article\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Author\"\n      }\n    },\n    \"source\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Originating news source or wire service\",\n      \"examples\": [\n        \"Bloomberg News\",\n        \"Bloomberg Opinion\",\n        \"Bloomberg Markets\",\n        \"Bloomberg Businessweek\"\n      ]\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 639-1 language code of the article\",\n      \"pattern\": \"^[a-z]{2}$\",\n      \"examples\": [\"en\", \"ja\", \"zh\", \"de\", \"fr\"]\n    },\n    \"wordCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total word count of the article body\",\n      \"minimum\": 0\n    },\n    \"articleType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the article type\",\n      \"enum\": [\n        \"News\",\n        \"Analysis\",\n        \"Opinion\",\n        \"Feature\",\n        \"Breaking\",\n        \"Exclusive\",\n        \"Flash\",\n        \"Commentary\",\n        \"Research\",\n        \"Interview\"\
  ,\n        \"Press Release\"\n      ]\n    },\n    \"urgency\": {\n      \"type\": \"string\",\n      \"description\": \"News urgency classification reflecting the BLPAPI NEWS_STORY_URGENCY field\",\n      \"enum\": [\n        \"Flash\",\n        \"Bulletin\",\n        \"Urgent\",\n        \"Normal\",\n        \"Background\"\n      ]\n    },\n    \"topics\": {\n      \"type\": \"array\",\n      \"description\": \"Bloomberg topic codes and categories associated with the article\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Topic\"\n      }\n    },\n    \"securities\": {\n      \"type\": \"array\",\n      \"description\": \"Securities mentioned in or related to the article, referenced by Bloomberg identifiers\",\n      \"items\": {\n        \"$ref\": \"#/$defs/SecurityReference\"\n      }\n    },\n    \"regions\": {\n      \"type\": \"array\",\n      \"description\": \"Geographic regions relevant to the article\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"\
  examples\": [\n        [\"US\", \"EMEA\", \"APAC\", \"LATAM\"]\n      ]\n    },\n    \"sectors\": {\n      \"type\": \"array\",\n      \"description\": \"Industry sectors relevant to the article content\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"Technology\", \"Finance\", \"Energy\", \"Healthcare\"]\n      ]\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Free-form tags or keywords associated with the article\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"media\": {\n      \"type\": \"array\",\n      \"description\": \"Associated multimedia content such as images, videos, or charts\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MediaAttachment\"\n      }\n    },\n    \"relatedStories\": {\n      \"type\": \"array\",\n      \"description\": \"References to related Bloomberg news stories\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n\
  \          \"storyId\": {\n            \"type\": \"string\",\n            \"description\": \"Bloomberg story identifier of the related article\"\n          },\n          \"headline\": {\n            \"type\": \"string\",\n            \"description\": \"Headline of the related article\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL of the related article\"\n          }\n        }\n      }\n    },\n    \"copyright\": {\n      \"type\": \"string\",\n      \"description\": \"Copyright notice for the article content\",\n      \"examples\": [\"Copyright 2026 Bloomberg L.P.\"]\n    }\n  },\n  \"$defs\": {\n    \"Author\": {\n      \"type\": \"object\",\n      \"description\": \"A Bloomberg news article author or contributor\",\n      \"required\": [\"name\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Full name of the author\"\n     \
  \   },\n        \"email\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"email\",\n          \"description\": \"Author's email address\"\n        },\n        \"bio\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Short biographical description of the author\"\n        },\n        \"url\": {\n          \"type\": [\"string\", \"null\"],\n          \"format\": \"uri\",\n          \"description\": \"URL to the author's Bloomberg profile\"\n        }\n      }\n    },\n    \"Topic\": {\n      \"type\": \"object\",\n      \"description\": \"Bloomberg topic classification for news categorization\",\n      \"required\": [\"code\"],\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg topic code\",\n          \"examples\": [\"MARKETS\", \"ECO\", \"POL\", \"TECH\", \"CORP\", \"CMDTY\", \"FX\", \"FI\"]\n        },\n        \"name\": {\n          \"type\": \"string\",\n       \
  \   \"description\": \"Human-readable topic name\",\n          \"examples\": [\"Markets\", \"Economics\", \"Politics\", \"Technology\", \"Corporate News\", \"Commodities\", \"Foreign Exchange\", \"Fixed Income\"]\n        }\n      }\n    },\n    \"SecurityReference\": {\n      \"type\": \"object\",\n      \"description\": \"A reference to a financial security mentioned in the article, using Bloomberg security identification conventions\",\n      \"properties\": {\n        \"ticker\": {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg ticker symbol in TICKER MARKET_SECTOR format\",\n          \"examples\": [\"AAPL US Equity\", \"IBM US Equity\", \"VOD LN Equity\"]\n        },\n        \"figi\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Financial Instrument Global Identifier (FIGI)\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Security display name\"\n        },\n        \"assetClass\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Bloomberg asset class classification\",\n          \"enum\": [\n            \"Equity\",\n            \"Fixed Income\",\n            \"Commodity\",\n            \"Currency\",\n            \"Index\",\n            \"Fund\",\n            \"Mortgage\",\n            \"Municipal\",\n            \"Preferred\",\n            \"Money Market\"\n          ]\n        }\n      }\n    },\n    \"MediaAttachment\": {\n      \"type\": \"object\",\n      \"description\": \"Multimedia content associated with the article\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Type of media content\",\n          \"enum\": [\"Image\", \"Video\", \"Chart\", \"Infographic\", \"Audio\"]\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL of the media asset\"\n        },\n        \"caption\": {\n          \"type\"\
  : [\"string\", \"null\"],\n          \"description\": \"Caption or description for the media asset\"\n        },\n        \"credit\": {\n          \"type\": [\"string\", \"null\"],\n          \"description\": \"Attribution credit for the media asset\"\n        },\n        \"mimeType\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the media content\",\n          \"examples\": [\"image/jpeg\", \"video/mp4\", \"image/png\"]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bloomberg-news/refs/heads/main/json-schema/bloomberg-news-article-schema.json
tags:
- Analytics
- Business Intelligence
- Financial Services
- Market Data
- News
title: Bloomberg News Article
---
