---
swagger: "2.0"
x-collection-name: Weather Underground
x-complete: 1
info:
  title: Weather Underground
  description: get-forecast-and-weather-data-with-complete-geolocation-services-global-coverage-and-more-
  version: 1.0.0
host: api.wunderground.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{key}/forecast/q/CA/San_Francisco.json:
    get:
      summary: Get Key Forecast Q Ca San Francisco
      description: This example will return the 3 Day Forecast Summary for San Francisco,
        California
      operationId: Get_forecast3_example_
      x-api-path-slug: keyforecastqcasan-francisco-json-get
      parameters:
      - in: path
        name: city
        description: The city
        type: string
        format: string
      - in: path
        name: state
        description: The state
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Key
      - Forecast
      - Q
      - CA
      - San
      - Francisco
      - Json
  /{key}/conditions/forecast/lang:FR/q/France/Paris.json:
    get:
      summary: Get Key Conditions Forecast Lang Fr Q France Paris
      description: This example will return Current Conditions and a 3 day simple
        Forecast for Paris France in French. See documentation page for full list
        of language code options.
      operationId: Get_French_example_
      x-api-path-slug: keyconditionsforecastlangfrqfranceparis-json-get
      parameters:
      - in: path
        name: city
        description: The city
        type: string
        format: string
      - in: path
        name: country
        description: The country
        type: string
        format: string
      - in: path
        name: language
        description: The language
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Key
      - Conditions
      - Forecast
      - Lang:FR
      - Q
      - France
      - Paris
      - Json
  /{key}/conditions/forecast/lang:SP/q/Spain/Alicante.json:
    get:
      summary: Get Key Conditions Forecast Lang Sp Q Spain Alicante
      description: This example will return Current Conditions and a 3 day simple
        Forecast for Alicante, Spain in Spanish. See documentation page for full list
        of language code options.
      operationId: Get_Spanish_example_
      x-api-path-slug: keyconditionsforecastlangspqspainalicante-json-get
      parameters:
      - in: path
        name: city
        description: The city
        type: string
        format: string
      - in: path
        name: country
        description: The country
        type: string
        format: string
      - in: path
        name: language
        description: The language
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Key
      - Conditions
      - Forecast
      - Lang:SP
      - Q
      - Spain
      - Alicante
      - Json
  /{key}/geolookup/conditions/forecast/q/CA/San_Francisco.json:
    get:
      summary: Get Key Geolookup Conditions Forecast Q Ca San Francisco
      description: This example will return the geographical, current conditions and
        3 day forecast summary for San Francisco, California
      operationId: Get_Geolocate_current_forecast_example_
      x-api-path-slug: keygeolookupconditionsforecastqcasan-francisco-json-get
      parameters:
      - in: path
        name: city
        description: The city
        type: string
        format: string
      - in: path
        name: state
        description: The state
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Key
      - Geolookup
      - Conditions
      - Forecast
      - Q
      - CA
      - San
      - Francisco
      - Json
---