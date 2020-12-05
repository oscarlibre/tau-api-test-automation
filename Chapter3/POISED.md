# Lesson 3: POISED API testing strategy 

![](https://testautomationu.applitools.com/course12/lesson3.0-coverimage.png)

#### What we want of our APIs 
- To be *CORRECT* in that they are fulfilling their contract correctly.
- APIs that *PROVIDE VALUE* for the developers creating applications.
- APIs that are *INTUITIVE* to use.
  
#### POISED
- Heuristic for helping with test coverage.
- POISED stands for Parameters, Output, Interop, Security, Errors, and Data.

##### Parameters
- The parameters represent the input for your API.
- Perform classic boundary style testing on the parameters.
- The other thing to look at is whether an invalid value causes a problem.
- Find out how the API reacts under different conditions.

##### Output
- The output could be not only the response itself, but the status code, the logging, or perhaps any kind of monitoring information that you want to send.
- The headers can change output format (e.g JSON, XML, YAML, etc..)
- The API can provide not only the right answer, it's being able to give clues to the developer when things aren't quite right.

##### Interoperability
- An API is all about communication. It needs to be communicating in a way that other services or other applications can get the information that they need.
- Think about how your parameters are actually formatted and how picky are they about the format (e.g Dates and Currencies)
- Basically, you need to communicate about the kind of communication your API is doing
- If you have good interoperability, then it's a lot easier for people to use your API and it makes it a better API.

##### Security
- Having security at the UI level is good, but it's not enough to secure your API.
- Encryption
- Authentication
- Restrict access to your system to a limited number of messages per second.
- Data validation, using schema validation and check that your parameters are what they should be (string, integer…) to prevent any SQL injection or XML bomb. ![extra source]("https://apifriends.com/api-security/api-security-best-practices/")

##### Errors
- Errors and exception handling
- Bad information can be passed into a request, and the service needs to be able to handle that information gracefully, without crashing.
- Proper communication of the erroneous result (e.g mismatch between our status and the actual problem of having bad credentials).
- API should be able to determine which part of the request is bad and be able to communicate that somehow either through an exception or perhaps in a debug log.

##### Data
- Making sure that the data is being handled properly is a very important part of testing APIs.
- It's not enough to just say, "Well, we got a 200 OK and a response back." 
- Don't just trust that the response is doing what it's doing. Actually make sure that the data is where it should be.
- Another important part of data handling is making sure that you're collecting the data that you need to have.
- Scalability, this is a data-related challenge that's very important to consider in any API that's going to have more than one or two users or will it be able to perform all the operations quickly enough


![Source](https://testautomationu.applitools.com/exploring-service-apis-through-test-automation/chapter3.0.html)
   
