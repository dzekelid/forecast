{
  "info": {
    "name": "Weatherbit Get Forecast Daily Lat & Lon",
    "_postman_id": "a7320b38-7b40-4d7a-9e9c-c30ab12538b5",
    "description": "**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast, where each point represents one day (24hr) period. Every point has a datetime string in the format \"YYYY-MM-DD\". One day begins at 00:00 UTC, and ends at 23:59 UTC.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "weather",
      "item": [
        {
          "id": "53b105de-0efc-4e5c-8cee-526171988073",
          "name": "required-basic-plan-or-higher-returns-a-daily-forecast-where-each-point-represents-one-day-24hr-peri",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.weatherbit.io",
              "path": [
                "v2.0",
                "forecast/daily?lat=:lat&lon=:lon"
              ],
              "query": [
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "days",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "lang",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "units",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "lat",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "lon",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "**(REQUIRED: Basic Plan or Higher)** Returns a daily forecast, where each point represents one day (24hr) period"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3608d2a-3b90-49fc-b96a-b8d618569b3f"
            }
          ]
        }
      ]
    }
  ]
}