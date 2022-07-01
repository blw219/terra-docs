[__Back to home__](../index.md)

# Ethical Consequences

## Data

Terra provides two main methods of receiving data from your users. HTTP requests and webhook pushes.
HTTP requests allow you to manually request for recent or historical data for any of your users at any time. You should note however that SDK integrations do not support retreival of data through HTTP requests and the requests should instead be performed on the device. See HTTP Requests for more.
Webhooks allow you immediate access to new user data. We send a POST request to your configured webhook URL whenever we are notified or detect new data is available for any of your users. All you need to do is listen for these pushes and process them on your backend. See Webhooks for more.


When handling personal data care must be taken to ensure that it is kept securely and not used for purposes not agreed to by the user.
We must ensure that we have authorisation to access someones data and information.


## Security

Data is anonymous never stored and securely transferred using HMAC payload integrity verification.

## Suggestions

Our goal is to give a better insight on the user health. Using terra's unified API we were able to bring different data together in want place and create a deeper analysis.
When connecting to the dashboard the user has data on his activity , sleep and nutrition . From this data we give suggestions combining all three factors.
 For exemple if the sleep data shows an irregular pattern we check the amount of calories consumed is greater than the recommended 2500 per day and the amount of calories burned is less than 500 the dashboarrd will pop a message saying "A more active routine can help improve qualiity and duration of sleep. 
 This allows the user to understand how performance nutrition and sleep can impact one another and how to have a good health balance using the suggestions given.


