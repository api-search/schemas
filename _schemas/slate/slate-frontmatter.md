---
description: YAML frontmatter configuration for Slate API documentation pages. Slate is a static site generator for beautiful three-panel API documentation written in Markdown. The frontmatter in each index.html.md file controls the page title, language tabs, table of contents, included files, search behavior, meta tags, and other display options.
layout: schema
name: Slate Frontmatter Configuration
properties_list:
- description: The title of the API documentation page, displayed in the browser tab and page header.
  name: title
  type: string
- description: List of programming languages for which code samples are shown as switchable tabs in the right panel. Must be valid Rouge lexer names (see https://github.com/rouge-ruby/rouge/wiki/List-of-supported-la
  name: language_tabs
  type: array
- description: HTML anchor elements or plain text strings displayed at the bottom of the table of contents sidebar.
  name: toc_footers
  type: array
- description: List of Markdown include file names (without extension) to be concatenated into the documentation page. Files must exist in the source/includes/ directory.
  name: includes
  type: array
- description: Whether to enable the full-text search functionality in the documentation sidebar. When true, a search box appears above the table of contents.
  name: search
  type: boolean
- description: Whether to enable copy-to-clipboard buttons on code sample blocks in the right panel.
  name: code_clipboard
  type: boolean
- description: The syntax highlighting theme to use for code blocks. Slate uses Rouge for syntax highlighting.
  name: highlight_theme
  type: string
- description: List of HTML meta tag definitions to be injected into the documentation page head element for SEO and social sharing.
  name: meta
  type: array
- description: Optional logo image configuration for the sidebar.
  name: logo
  type: object
provider_name: Slate
provider_slug: slate
schema_file: json-schema/slate-frontmatter-schema.json
slug: slate-frontmatter
source_filename: slate-frontmatter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://apievangelist.com/schemas/slate/slate-frontmatter.json\",\n  \"title\": \"Slate Frontmatter Configuration\",\n  \"description\": \"YAML frontmatter configuration for Slate API documentation pages. Slate is a static site generator for beautiful three-panel API documentation written in Markdown. The frontmatter in each index.html.md file controls the page title, language tabs, table of contents, included files, search behavior, meta tags, and other display options.\",\n  \"type\": \"object\",\n  \"required\": [\"title\"],\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the API documentation page, displayed in the browser tab and page header.\",\n      \"minLength\": 1,\n      \"examples\": [\"API Reference\", \"Kittn API Documentation\"]\n    },\n    \"language_tabs\": {\n      \"type\": \"array\",\n      \"description\": \"List\
  \ of programming languages for which code samples are shown as switchable tabs in the right panel. Must be valid Rouge lexer names (see https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers).\",\n      \"items\": {\n        \"$ref\": \"#/$defs/LanguageTab\"\n      },\n      \"minItems\": 1,\n      \"examples\": [\n        [\"shell\", \"ruby\", \"python\", \"javascript\"],\n        [{\"shell\": \"cURL\"}, {\"javascript\": \"JS\"}]\n      ]\n    },\n    \"toc_footers\": {\n      \"type\": \"array\",\n      \"description\": \"HTML anchor elements or plain text strings displayed at the bottom of the table of contents sidebar.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"An HTML string or plain text entry shown in the TOC footer area.\"\n      },\n      \"examples\": [\n        [\"<a href='#'>Sign Up for a Developer Key</a>\", \"<a href='https://github.com/slatedocs/slate'>Documentation Powered by Slate</a>\"]\n      ]\n    },\n\
  \    \"includes\": {\n      \"type\": \"array\",\n      \"description\": \"List of Markdown include file names (without extension) to be concatenated into the documentation page. Files must exist in the source/includes/ directory.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"The filename (without extension) of a Markdown file in the includes/ directory.\",\n        \"pattern\": \"^[a-zA-Z0-9_-]+$\"\n      },\n      \"examples\": [\n        [\"errors\", \"authentication\", \"pagination\"]\n      ]\n    },\n    \"search\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable the full-text search functionality in the documentation sidebar. When true, a search box appears above the table of contents.\",\n      \"default\": false\n    },\n    \"code_clipboard\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable copy-to-clipboard buttons on code sample blocks in the right panel.\",\n      \"default\": false\n\
  \    },\n    \"highlight_theme\": {\n      \"type\": \"string\",\n      \"description\": \"The syntax highlighting theme to use for code blocks. Slate uses Rouge for syntax highlighting.\",\n      \"examples\": [\"monokai_sublime\"]\n    },\n    \"meta\": {\n      \"type\": \"array\",\n      \"description\": \"List of HTML meta tag definitions to be injected into the documentation page head element for SEO and social sharing.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MetaTag\"\n      },\n      \"examples\": [\n        [{\"name\": \"description\", \"content\": \"Documentation for the Example API\"}]\n      ]\n    },\n    \"logo\": {\n      \"$ref\": \"#/$defs/LogoConfig\",\n      \"description\": \"Optional logo image configuration for the sidebar.\"\n    }\n  },\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"LanguageTab\": {\n      \"oneOf\": [\n        {\n          \"type\": \"string\",\n          \"description\": \"A Rouge lexer identifier used as both the tab identifier\
  \ and display label.\",\n          \"minLength\": 1,\n          \"examples\": [\"shell\", \"ruby\", \"python\", \"javascript\", \"java\", \"go\", \"csharp\", \"php\"]\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"A mapping of a Rouge lexer identifier to a custom display label for the tab.\",\n          \"minProperties\": 1,\n          \"maxProperties\": 1,\n          \"additionalProperties\": {\n            \"type\": \"string\",\n            \"description\": \"The human-readable display label for this language tab.\",\n            \"minLength\": 1\n          },\n          \"examples\": [\n            {\"shell\": \"cURL\"},\n            {\"javascript\": \"Node.js\"},\n            {\"csharp\": \"C#\"}\n          ]\n        }\n      ],\n      \"description\": \"A language tab entry, either a plain Rouge lexer name or a mapping from lexer name to display label.\"\n    },\n    \"MetaTag\": {\n      \"type\": \"object\",\n      \"description\": \"An HTML\
  \ meta tag to be injected into the documentation page head.\",\n      \"required\": [\"name\", \"content\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name attribute of the HTML meta tag.\",\n          \"examples\": [\"description\", \"keywords\", \"author\", \"robots\"]\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The content attribute of the HTML meta tag.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"LogoConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Logo image configuration for display in the documentation sidebar.\",\n      \"required\": [\"image\"],\n      \"properties\": {\n        \"image\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL or relative path to the logo image file.\"\n        },\n        \"link\": {\n          \"type\": \"string\",\n     \
  \     \"format\": \"uri\",\n          \"description\": \"Optional URL to navigate to when the logo is clicked.\"\n        }\n      },\n      \"additionalProperties\": false\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/slate/refs/heads/main/json-schema/slate-frontmatter-schema.json
tags:
- API Documentation
- Developer Tools
- Documentation
- Markdown
- Ruby
- Static Site Generator
- Three-Panel
title: Slate Frontmatter Configuration
---
