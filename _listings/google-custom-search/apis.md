---
name: Google Custom Search
description: The JSON/Atom Custom Search API lets you develop websites and applications
  to retrieve and display search results from Google Custom Search programmatically.
  With this API, you can use RESTful requests to get either web search or image search
  results in JSON or Atom format.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-custom-search.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Stack Network
- Search
- Google APIs
created: "2018-03-24"
modified: "2018-03-24"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/google-custom-search/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google Custom Search JSON/Atom API
  description: The JSON/Atom Custom Search API lets you develop websites and applications
    to retrieve and display search results from Google Custom Search programmatically
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-custom-search.png
  humanURL: ""
  baseURL: ://www.googleapis.com//customsearch
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/google-custom-search/v1-get.md
- name: Google Custom Search JSON/Atom API Search
  description: Returns metadata about the search performed, metadata about the custom
    search engine used for the search, and the search results.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-custom-search.png
  humanURL: ""
  baseURL: http:://www.googleapis.com//customsearch
  tags: Search
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/google-custom-search/v1-get.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/search/master/_listings/google-custom-search/v1-get-postman.md
x-common:
- type: x-blog
  url: https://customsearch.googleblog.com/
- type: x-blog-rss
  url: http://googlecustomsearch.blogspot.in/atom.xml
- type: x-code
  url: https://developers.google.com/custom-search/json-api/v1/libraries
- type: x-twitter
  url: https://twitter.com/googlecse
- type: x-blog
  url: https://customsearch.googleblog.com/
- type: x-blog-rss
  url: http://googlecustomsearch.blogspot.in/atom.xml
- type: x-code
  url: https://developers.google.com/custom-search/json-api/v1/libraries
- type: x-twitter
  url: https://twitter.com/googlecse
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---