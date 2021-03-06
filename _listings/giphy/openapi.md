swagger: "2.0"
x-collection-name: Giphy
x-complete: 1
info:
  title: Giphy
  description: natively-embed-all-the-best-features-of-the-worlds-largest-and-most-powerful-gif-library-into-your-app-
  termsOfService: https://developers.giphy.com/
  version: v1
host: api.giphy.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gifs/search:
    get:
      summary: Search GIFs
      description: Search all GIPHY GIFs for a word or phrase. Punctuation will be
        stripped and ignored.  Use a plus or url encode for phrases. Example paul+rudd,
        ryan+gosling or american+psycho.
      operationId: searchGifs
      x-api-path-slug: gifssearch-get
      parameters:
      - in: query
        name: No Name
      responses:
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Gifs
      - Search
  /stickers/search:
    get:
      summary: Search Stickers
      description: Replicates the functionality and requirements of the classic GIPHY
        search, but returns animated stickers rather than GIFs.
      operationId: searchStickers
      x-api-path-slug: stickerssearch-get
      parameters:
      - in: query
        name: No Name
      responses:
        100:
          description: Invalid API Key - The API key passed was not valid or has expired
        105:
          description: Service currently unavailable - The requested service is temporarily
            unavailable
        106:
          description: Write operation failed - The requested operation failed due
            to a temporary issue
        111:
          description: Format "xxx" not found - The requested response format was
            not found
        112:
          description: Method "xxx" not found - The requested method was not found
        114:
          description: Invalid SOAP envelope - The SOAP envelope send in the request
            could not be parsed
        115:
          description: Invalid XML-RPC Method Call - The XML-RPC request document
            could not be parsed
        116:
          description: Bad URL found - One or more arguments contained a URL that
            has been used for abuse on Flickr
      tags:
      - Stickers
      - Search