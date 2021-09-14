# Errors

Squiry uses conventional HTTP response codes to indicate the success or failure of an API request. In general: Codes in the `2xx`range indicate success. Codes in the `4xx` range indicate an error that failed given the information provided \(e.g., a required parameter was omitted, a charge failed, etc.\). Codes in the `5xx` range indicate an error with Squiry's servers \(these are rare\).

| Code    | Description                                                                                                                                |
| :------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| 200     | Everything worked as expected.                                                                                                             |
| 400     | The request was unacceptable, often due to missing a required parameter.                                                                   |
| 401     | No valid API key provided.                                                                                                                 |
| 404     | The requested resource doesn't exist.                                                                                                      |
| 500-504 | Something went wrong on Squiry's end. These are rare and if they happen, please [contact us](https://smartsquiry.com/support) immediately. |
