swagger: "2.0"
x-collection-name: Weatherbit.io
x-complete: 1
info:
  title: Weatherbit
  description: this-is-the-documentation-for-the-weatherbit-api---the-base-url-for-the-api-is-httpapi-weatherbit-iov2-0httpapi-weatherbit-iov2-0-or-httpsapi-weatherbit-iov2-0httpapi-weatherbit-iov2-0--below-is-the-swagger-ui-documentation-for-the-api--all-api-requests-require-the-key-parameter---------an-example-for-a-5-day-forecast-for-london-uk-would-be-httpapi-weatherbit-iov2-0forecast3hourlycitylondoncountryuk
  version: 2.0.0
host: api.weatherbit.io
basePath: /v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /forecast/3hourly?city={city}&country={country}:
    get:
      summary: Get Forecast 3hourly City & Country
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - City
      - City
      - '&country'
      - Country
  /forecast/3hourly?city_id={city_id}:
    get:
      summary: Get Forecast 3hourly City
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - City
      - ""
      - City
  /forecast/3hourly?ip={ip}:
    get:
      summary: Get Forecast 3hourly IP
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: path
        name: ip
        description: IP address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - Ip
      - Ip
  /forecast/3hourly?lat={lat}&lon={lon}:
    get:
      summary: Get Forecast 3hourly Lat & Lon
      description: Returns a 3-hourly forecast, where each point represents a three
        hour   period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour---period-every-point-has-a-datet
      x-api-path-slug: forecast3hourlylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - Lat
      - Lat
      - '&lon'
      - Lon
  /forecast/3hourly?postal_code={postal_code}:
    get:
      summary: Get Forecast 3hourly Postla Code Code
      description: Returns a 3-hourly forecast, where each point represents a three
        hour period. Every point has a datetime string in the format "YYYY-MM-DD:HH".
        Time is UTC.
      operationId: returns-a-3hourly-forecast-where-each-point-represents-a-three-hour-period-every-point-has-a-datetim
      x-api-path-slug: forecast3hourlypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - 3hourly
      - Postal
      - Code
      - Postal
      - Code
  /forecast/daily?city={city}&country={country}:
    get:
      summary: Get Forecast Daily City & Country
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC. Accepts a city in the format of City,ST or City. The state, and
        country parameters can be provided to make the search more accurate.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - City
      - City
      - '&country'
      - Country
  /forecast/daily?city_id={city_id}:
    get:
      summary: Get Forecast Daily City
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - City
      - ""
      - City
  /forecast/daily?ip={ip}:
    get:
      summary: Get Forecast Daily IP
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: path
        name: ip
        description: IP address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - Ip
      - Ip
  /forecast/daily?lat={lat}&lon={lon}:
    get:
      summary: Get Forecast Daily Lat & Lon
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - Lat
      - Lat
      - '&lon'
      - Lon
  /forecast/daily?postal_code={postal_code}:
    get:
      summary: Get Forecast Daily Postla Code Code
      description: '**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast,
        where each point represents one day (24hr) period. Every point has a datetime
        string in the format "YYYY-MM-DD". One day begins at 00:00 UTC, and ends at
        23:59 UTC.'
      operationId: required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri
      x-api-path-slug: forecastdailypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Daily
      - Postal
      - Code
      - Postal
      - Code
  /forecast/hourly?city={city}&country={country}:
    get:
      summary: Get Forecast Hourly City & Country
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour   period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC. Accepts a city in the format
        of City,ST or City. The state, and country parameters can be provided to make
        the search more accurate.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlycitycitycountrycountry-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city
        description: City search
      - in: path
        name: country
        description: Country Code (2 letter)
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: state
        description: Full name of state
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - City
      - City
      - '&country'
      - Country
  /forecast/hourly?city_id={city_id}:
    get:
      summary: Get Forecast Hourly City
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour   period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlycity-idcity-id-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: path
        name: city_id
        description: City ID
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - City
      - ""
      - City
  /forecast/hourly?ip={ip}:
    get:
      summary: Get Forecast Hourly IP
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlyipip-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: days
        description: Number of days to return
      - in: query
        name: hours
        description: Number of hours to return
      - in: path
        name: ip
        description: IP address, or auto
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - Ip
      - Ip
  /forecast/hourly?lat={lat}&lon={lon}:
    get:
      summary: Get Forecast Hourly Lat & Lon
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlylatlatlonlon-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: lat
        description: Latitude component of location
      - in: path
        name: lon
        description: Longitude component of location
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - Lat
      - Lat
      - '&lon'
      - Lon
  /forecast/hourly?postal_code={postal_code}:
    get:
      summary: Get Forecast Hourly Postla Code Code
      description: '**(REQUIRED: Developer Plan or Higher)** Returns an hourly forecast,
        where each point represents a one hour   period. Every point has a datetime
        string in the format "YYYY-MM-DD:HH". Time is UTC.'
      operationId: required-developer-plan-or-higher-returns-an-hourly-forecast-where-each-point-represents-a-one-hour-
      x-api-path-slug: forecasthourlypostal-codepostal-code-get
      parameters:
      - in: query
        name: callback
        description: Wraps return in jsonp callback
      - in: query
        name: country
        description: Country Code (2 letter)
      - in: query
        name: hours
        description: Number of hours to return
      - in: query
        name: key
        description: Your registered API key
      - in: query
        name: lang
        description: 'Language (Default: English) See language field description'
      - in: path
        name: postal_code
        description: Postal Code
      - in: query
        name: units
        description: Convert to units
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Forecast
      - Hourly
      - Postal
      - Code
      - Postal
      - Code