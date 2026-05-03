---
description: Configuration options for the Nextra Next.js plugin, passed as the argument to the nextra() function in next.config. Controls MDX compilation, search, syntax highlighting, LaTeX, image optimization, and i18n behavior.
layout: schema
name: Nextra Configuration
properties_list:
- description: Enable the copy button for all code blocks by default, without needing to set copy=true in the code block metadata. Individual blocks can still disable it with copy=false.
  name: defaultShowCopyCode
  type: boolean
- description: Option to enable search functionality powered by Pagefind. When enabled, sets the data-pagefind-body attribute on the main element. Can be a boolean or an object controlling code block indexing.
  name: search
  type: object
- description: Automatically optimize static image imports used with standard Markdown image syntax, e.g. ![alt](/image.png). Uses next/image under the hood.
  name: staticImage
  type: boolean
- description: Adds estimated reading time of .md and .mdx files using the reading-time package. The value is injected into the page front matter under the readingTime key.
  name: readingTime
  type: boolean
- description: Enable LaTeX rendering. Supports KaTeX (server-side, fast) and MathJax (browser-side, more complete). Pass true to use KaTeX with defaults.
  name: latex
  type: object
- description: Enable or disable syntax highlighting for code blocks via Rehype Pretty Code.
  name: codeHighlight
  type: boolean
- description: ''
  name: mdxOptions
  type: object
- description: Allows you to whitelist HTML elements to be replaced with components defined in the mdx-components.js file. By default only details and summary are replaced.
  name: whiteListTagsStyling
  type: array
- description: Serve .md and .mdx files from the content directory at a custom path instead of the root (/). Must begin with / and must not end with /.
  name: contentDirBasePath
  type: string
- description: Prefixes locale to all links in the page map information. Useful for i18n setups that do not use Nextra's middleware function.
  name: unstable_shouldAddLocaleToLinks
  type: boolean
provider_name: Nextra
provider_slug: nextra
schema_file: json-schema/nextra-config-schema.json
slug: nextra-config
source_filename: nextra-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://nextra.site/schemas/nextra/nextra-config.json\",\n  \"title\": \"Nextra Configuration\",\n  \"description\": \"Configuration options for the Nextra Next.js plugin, passed as the argument to the nextra() function in next.config. Controls MDX compilation, search, syntax highlighting, LaTeX, image optimization, and i18n behavior.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"defaultShowCopyCode\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable the copy button for all code blocks by default, without needing to set copy=true in the code block metadata. Individual blocks can still disable it with copy=false.\"\n    },\n    \"search\": {\n      \"description\": \"Option to enable search functionality powered by Pagefind. When enabled, sets the data-pagefind-body attribute on the main element. Can be a boolean or an object controlling code block indexing.\",\n     \
  \ \"oneOf\": [\n        {\n          \"type\": \"boolean\",\n          \"description\": \"Pass true to enable search with defaults, false to disable.\"\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"Fine-grained search configuration.\",\n          \"required\": [\"codeblocks\"],\n          \"properties\": {\n            \"codeblocks\": {\n              \"type\": \"boolean\",\n              \"description\": \"Whether to index code blocks. When false, adds data-pagefind-ignore=\\\"all\\\" to all pre elements.\"\n            }\n          },\n          \"additionalProperties\": false\n        }\n      ],\n      \"default\": { \"codeblocks\": false }\n    },\n    \"staticImage\": {\n      \"type\": \"boolean\",\n      \"description\": \"Automatically optimize static image imports used with standard Markdown image syntax, e.g. ![alt](/image.png). Uses next/image under the hood.\",\n      \"default\": true\n    },\n    \"readingTime\": {\n      \"type\"\
  : \"boolean\",\n      \"description\": \"Adds estimated reading time of .md and .mdx files using the reading-time package. The value is injected into the page front matter under the readingTime key.\"\n    },\n    \"latex\": {\n      \"description\": \"Enable LaTeX rendering. Supports KaTeX (server-side, fast) and MathJax (browser-side, more complete). Pass true to use KaTeX with defaults.\",\n      \"oneOf\": [\n        {\n          \"type\": \"boolean\",\n          \"description\": \"Pass true to enable KaTeX with default options.\"\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"Use MathJax renderer with optional configuration.\",\n          \"required\": [\"renderer\"],\n          \"properties\": {\n            \"renderer\": {\n              \"type\": \"string\",\n              \"const\": \"mathjax\",\n              \"description\": \"Use the MathJax renderer.\"\n            },\n            \"options\": {\n              \"$ref\": \"#/$defs/MathJaxOptions\"\
  \n            }\n          },\n          \"additionalProperties\": false\n        },\n        {\n          \"type\": \"object\",\n          \"description\": \"Use KaTeX renderer with optional configuration.\",\n          \"required\": [\"renderer\"],\n          \"properties\": {\n            \"renderer\": {\n              \"type\": \"string\",\n              \"const\": \"katex\",\n              \"description\": \"Use the KaTeX renderer.\"\n            },\n            \"options\": {\n              \"type\": \"object\",\n              \"description\": \"KaTeX options. See https://katex.org/docs/options.html.\"\n            }\n          },\n          \"additionalProperties\": false\n        }\n      ]\n    },\n    \"codeHighlight\": {\n      \"type\": \"boolean\",\n      \"description\": \"Enable or disable syntax highlighting for code blocks via Rehype Pretty Code.\",\n      \"default\": true\n    },\n    \"mdxOptions\": {\n      \"$ref\": \"#/$defs/MdxOptions\"\n    },\n    \"whiteListTagsStyling\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"description\": \"HTML tag name to allow styling override via mdx-components.js.\"\n      },\n      \"description\": \"Allows you to whitelist HTML elements to be replaced with components defined in the mdx-components.js file. By default only details and summary are replaced.\"\n    },\n    \"contentDirBasePath\": {\n      \"type\": \"string\",\n      \"pattern\": \"^/\",\n      \"description\": \"Serve .md and .mdx files from the content directory at a custom path instead of the root (/). Must begin with / and must not end with /.\",\n      \"default\": \"/\"\n    },\n    \"unstable_shouldAddLocaleToLinks\": {\n      \"type\": \"boolean\",\n      \"description\": \"Prefixes locale to all links in the page map information. Useful for i18n setups that do not use Nextra's middleware function.\",\n      \"default\": false\n    }\n  },\n  \"additionalProperties\": false,\n  \"$defs\": {\n    \"MathJaxOptions\"\
  : {\n      \"type\": \"object\",\n      \"description\": \"Configuration options for the MathJax renderer.\",\n      \"properties\": {\n        \"src\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"URL for MathJax CDN. Defaults to https://cdnjs.cloudflare.com.\"\n        },\n        \"config\": {\n          \"type\": \"object\",\n          \"description\": \"MathJax 3 configuration object. See https://docs.mathjax.org/en/latest/options/index.html.\"\n        }\n      },\n      \"additionalProperties\": false\n    },\n    \"MdxOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Options controlling the MDX compilation pipeline.\",\n      \"properties\": {\n        \"rehypePlugins\": {\n          \"type\": \"array\",\n          \"description\": \"List of rehype plugins to apply during MDX compilation.\",\n          \"items\": {}\n        },\n        \"remarkPlugins\": {\n          \"type\": \"array\",\n          \"description\"\
  : \"List of remark plugins to apply during MDX compilation.\",\n          \"items\": {}\n        },\n        \"recmaPlugins\": {\n          \"type\": \"array\",\n          \"description\": \"List of recma plugins to apply. This is a new ecosystem for transforming esast (JavaScript AST) trees, currently in beta.\",\n          \"items\": {}\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"enum\": [\"detect\", \"mdx\", \"md\"],\n          \"description\": \"Format of the file. 'md' treats as markdown, 'mdx' treats as MDX, 'detect' auto-detects based on file extension.\",\n          \"default\": \"detect\"\n        },\n        \"rehypePrettyCodeOptions\": {\n          \"type\": \"object\",\n          \"description\": \"Configuration options for Rehype Pretty Code syntax highlighting. See https://github.com/rehype-pretty/rehype-pretty-code.\"\n        }\n      },\n      \"additionalProperties\": false\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nextra/refs/heads/main/json-schema/nextra-config-schema.json
tags:
- Documentation
- MDX
- Next.js
- Open Source
- Static Site Generator
title: Nextra Configuration
---
