[__Back to home__](../index.md)

# Ethical Considerations

## Data

Terra provides two main methods of receiving data from your users. HTTP requests and webhook pushes.
HTTP requests allow you to manually request for recent or historical data for any of your users at any time. You should note however that SDK integrations do not support retreival of data through HTTP requests and the requests should instead be performed on the device. See HTTP Requests for more.
Webhooks allow you immediate access to new user data. We send a POST request to your configured webhook URL whenever we are notified or detect new data is available for any of your users. All you need to do is listen for these pushes and process them on your backend. See Webhooks for more.

When handling personal data care must be taken to ensure that it is kept securely and not used for purposes not agreed to by the user. We must ensure that we have authorisation to access someones data and information which is ensured by Terra's connection widget. Users' data should also never be given to third party sources unless we have the user's consent. Storing data can also be unethical without the user's consent which we do, however we also make sure to regularly delete data we have.


## Security

Data is anonymous never stored and securely transferred using HMAC payload integrity verification. It should be protected against any unauthorised individuls who try to gain access to user data. Another step taken to maintain anonymity is when the session is closed the session id, which is used to identify the user's wearable data in our database, is deleted so there is no way to link a user to their data after this as they will only be stored in the databasae as a session id number.

## Suggestions

Our goal is to give a better insight on the user health. Using terra's unified API we were able to bring different data together in want place and create a deeper analysis.
When connecting to the dashboard the user has data on his activity, sleep and nutrition. From this data we give suggestions combining all three factors.
 For example if the sleep data shows an irregular pattern we check the amount of calories consumed is greater than the recommended 2500 per day and the amount of calories burned is less than 500 the dashboarrd will pop a message saying "A more active routine can help improve quality and duration of sleep. 
 This allows the user to understand how performance nutrition and sleep can impact one another and how to have a good health balance using the suggestions given.

It is important to consider the responsibility shouldered when advising someone on how to live their life to improve their health. As a result, care has to be taken when crafting suggestions for users to ensure that they strike a balance between being constructive and helpful and not demeaning or demotivating. By doing so comments should be worded in a way that they do not cause any potential harm to mental health of a user by misunderstanding comments given on their data.

## Sustainability

As this project is centred around building a website the only sustainability considerations concern the energy required to run servers for the website and database as well as the space to store servers. These factors have been considered and acknowledged and we hope that energy is provided from renewable and sustainable sources.

