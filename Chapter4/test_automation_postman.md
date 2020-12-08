# Lesson 4: Test automation in Postman

![](https://testautomationu.applitools.com/course12/lesson4.1-coverimage.png)

#### Overview
- How to create effective test automation in Postman.
- How to use Postman snippets to create tests quickly, 
- Data generation through pre-request scripts, using variables in tests, 
- Test setup using the Postman createRequest API, 
- Installing and running the Newman tool, 
- Running a Postman collection in Jenkins and viewing the result.

#### Your first test

For example, here’s a basic test just to make sure that we got a 200 OK response.

```javascript
pm.test(“Status code is 200”, function () {
	pm.response.to.have.status(200);
});
```

![Source chapter 4.1](https://testautomationu.applitools.com/exploring-service-apis-through-test-automation/chapter4.1.html)

##### Data driven testing

- Run one test multiple times with different data variables.
- On this example we tested certain range of characters that you're supporting in your names (first and last name), to make sure that all those characters are supported in different tests.
- This ![CSV file]("https://github.com/oscarlibre/tau-api-test-automation/blob/main/Chapter4/names_data.csv") was loaded from the postman collection runner

![Source chapter 4.2](https://testautomationu.applitools.com/exploring-service-apis-through-test-automation/chapter4.2.html)
   
