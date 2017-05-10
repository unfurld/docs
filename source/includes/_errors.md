# Errors

The Kittn API uses the following error codes:


Error Code | Meaning
---------- | -------
400        | Bad Request. The JSON response will contain an `errors` parameter explaining the reason
404        | An endpoint matching the specified URL could not be found
405        | The endpoint doesn't support the HTTP method used
429        | You've hit rate limits, increase or try again later.
