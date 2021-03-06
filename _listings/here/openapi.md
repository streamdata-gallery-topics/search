swagger: "2.0"
x-collection-name: HERE
x-complete: 1
info:
  title: Weather API
  description: the-here-weather-api-provides-weather-forecasts-and-reports-on-current-weather-conditions-provides-information-on-severe-weather-alerts-provides-information-about-when-the-sun-and-moon-rise-and-set-and-the-phase-of-the-moonthis-example-set-works-with-version-1-2-4-or-higheradditional-information-can-be-found-on-developer-here-comhttpsdeveloper-here-comrestapisdocumentationweather
  version: 1.0.0
host: weather.cit.api.here.com
basePath: /weather/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /suggest:
    get:
      summary: Search Suggestions
      description: |-
        *Request a list of suggestions based on a partial query string*

        A suggestions request can be made using the `suggest` endpoint in the request URL and adding the `q` parameter with the partial query string. The focal point for the suggestion service is defined using the `at` parameter.



        * **at**  `latlng`
         \- Location of the central point for the places search.    e.g. `52.515,13.377`

        * **q**  `text`
         \- Free-form text containing the search term.    e.g. `restaurant` or `Brandenburger Tor`

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

        * **Accept**  `header`

          Format to request from the server
      operationId: SuggestGet
      x-api-path-slug: suggest-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: at
      - in: query
        name: q
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
        200:
          description: OK
      tags:
      - Search
      - Suggestions
  /discover/search:
    get:
      summary: One-Box Search
      description: |-
        *Request a list of nearby places based on a query string*

        A free-text places search can be made using the `discover/search` endpoint in the request URL and adding the `q` parameter with the query string. The focal point of the search is defined using the `at` parameter.



        * **at**  `latlng`
         \- Location of the central point for the places search.    e.g. `52.515,13.377`

        * **q**  `text`
         \- Free-form text containing the search term.    e.g. `restaurant` or `Brandenburger Tor`

        * **app_id**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_id` with every request.

        * **app_code**  `text`
         \- A 20 byte Base64 URL-safe encoded string used for the authentication of the client application.    You must include an `app_code` with every request.

        * **Accept**  `header`

          Format to request from the server
      operationId: DiscoverSearchGet
      x-api-path-slug: discoversearch-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: at
      - in: query
        name: q
      responses:
        200:
          description: OK
      tags:
      - One-Box
      - Search