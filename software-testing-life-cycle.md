# Agile Testing

Agile testing is the process of continuously testing to ensure a constant feedback loop throughout the development process. In Agile, testing is the responsibility of the entire team. This ongoing feedback loop informs the team how well the product is adapting to the business needs. Gone are the days that testing is done at the end.

The  entire team shares the responsibility of testing. “Quality” is injected into the entire team. Agile teams put quality first and by doing so, they’re able to work faster. It widens the throughout of the testing process and eliminates the testing bottleneck

```

1. Agile testing promotes collaboration. It emphasizes integrated teams, frequent releases,
and the ability to adapt to changing business requirements. It involves the entire team 
throughout the entire development lifecycle.

2. Agile testing shortens the feedback loop, and shorter feedback loops increase the team’s
agility.

3. Agile testing does not eliminate the need for a QA team though. It does not replace manual testing.
It means automated and manual testing is no longer only the responsibility of the QA team. 
QA and development can often pair together to conduct exploratory testing.


```



## Agile testing tools

We’ve put together a shortlist of tools that you may want to consider using to help with your testing efforts. Not all tools will work for every team and as with everything in agile, you should be constantly reviewing what tools you use and adapt them so that they continually meet both yours and the team’s needs.
Cross browser testing tools

### BrowserStack 

These days it is essential to test any website or online application on not just desktop browsers but also tablet and mobile platforms. BrowserStack allows you to start a live session on many devices and browsers directly from your browser.


## Litmus 

Emails often don’t appear as expected in email clients and testing all the different clients can mean a lot of wasted time setting up accounts and re-sending the same email. Litmus offers cross client testing for emails and will save you a huge amount of time.


### Selenium

### Test management

#### TestLodge 

Documenting your testing efforts is just as essential within an agile team as with other methodologies. Writing lightweight tests will allow you to adapt them over time and using a lightweight test management tool to help manage this process can not only keep you organized and be a huge time saver, but can also provide key reports and identify trends which can be used within you team retrospectives.
Defect tracking

### Trello 

Agile teams often work with lightweight boards, lists and cards and this is exactly what Trello provides. This lightweight tool can be used to track issues and allow your entire team to quickly see the progress in the same way that your scrum board works.
Pivotal Tracker – A similar concept to Trello which will allow you to track issues on a board as well as some additional functionality which will come in useful when working within an agile team.

### Communication

#### JIRA


#### Slack 

A real time messaging app for teams which allows you to bring all your communication into one place and cut down on all those emails.

#### Zoom 

Working in the same location is not always possible, you may have remote workers or your client may be the other side of the world. Zoom allows you to host video conferences on a lightweight system.

#### Other

LICEcap – Captures short recordings of your screen into a gif so you can upload them to either your test management or defect tracking tools to help explain any issues you find.

## Software Testing Life Cycle

What phases make up the software testing life cycle?

Phases of the software testing life cycle may very, but in general, they involve planning, preparing, conducting, and reporting. Lets take a close look at different parts of the software testing life cycle.


### Requirements Analysis

In this first phase of the software testing life cycle, the test team reviews any requirements documents and designs to determine what is testable. By studying the requirements, the testing teams gets an understanding of the scope of testing. This phase might involve conversations with developers, designers, and stakeholders.

### Test Planning

What to test, how the test needs to be done, and who’s going to test it… these are the things determined during the test planning phase. Once the requirements have been reviewed, it’s time to plan the testing project at a high level. A test plan document is created during this phase. This phase gets everyone on the same page as far as how the testing project will be approached.

### Test Case Development

The goal of this phase is to determine in detail “how” to test. Test cases should be written to guide the tester through each test. If old test cases are being used, make sure they are up to date. Many tests might require test data. Prepare any test data required to run tests during this phase so that the you don’t have to spend time doing this during the tests.

### Environment

The test environment is the configuration of software and/or hardware on which the testing team is to perform the tests. Without the test environment ready to go, you’re going to hit roadblocks. Make sure any test data necessary is entered into the system and ready to be used. It’s not uncommon for this phase to happen alongside the test case development phase.

### Test Execution

Now that the tests are ready to go and the environment is setup, it’s time to run the tests. Using the test cases, the tester executes each test, comparing the expected results to the actual results of each test and marking it as pass/fail/skip. If the test fails, the tester should document what actually happened during the test. This phase also involves the tester logging bugs in the designated bug tracking system (determined in the test plan phase).

### Test Reporting and Coverage

Once all the tests cases are ran, the test manager should confirm all required testing have been completed. This involves an analysis of defects found and other metrics such as how many passed/failed/skipped test cases. This final phase in the software testing life Cycle might also include a retrospective on the testing project/process. This allows the team to learn and improve for future testing projects.
Conclusion

In general, the software testing life Cycle involves planning, preparing, conducting, and reporting of tests. Some of the phases in the STLC are dependent on others, some can happen alongside each other. By understanding each phase in the STLC you can ensure your testing process is efficient and effective.


## Types of Tests


1. Functional Testing 

```
Regression 

Integration 

Smoke Testing

```

2. Browser Compatibility Testing.

3. Performance Testing.

4. Security Testing.

5. Production Monitoring.

6. Usability Testing.


## Web Application Testing Checklist:

Some or all of the following testing types may be performed depending on your web testing requirements.

1. Functionality Testing:

This is used to check if your product is as per the specifications you intended for it as well as the functional requirements you charted out for it in your developmental documentation. Testing Activities Included:

Test all links in your webpages are working correctly and make sure there are no broken links. Links to be checked will include -
```
	Outgoing links

	Internal links

	Anchor Links

	MailTo Links

```

Test Forms are working as expected. This will include -

```
Scripting checks on the form are working as expected. For example- if a user does not fill a mandatory field in a form an error message is shown.

Check default values are being populated

Once submitted, the data in the forms is submitted to a live database or is linked to a working email address

Forms are optimally formatted for better readability
```


Test Cookies are working as expected. Cookies are small files used by websites to primarily remember active user sessions so you do not need to log in every time you visit a website. Cookie Testing will include

```
Testing cookies (sessions) are deleted either when cache is cleared or when they reach their expiry.

Delete cookies (sessions) and test that login credentials are asked for when you next visit the site.

```


Test HTML and CSS to ensure that search engines can crawl your site easily. This will include

```
	Checking for Syntax Errors

	Readable Color Schemas

	Standard Compliance. Ensure standards such W3C, OASIS, IETF, ISO, ECMA, or WS-I are followed.
```


Test business workflow- This will include

```
	Testing your end - to - end workflow/ business scenarios which takes the user through a series of webpages to complete.

	Test negative scenarios as well, such that when a user executes an unexpected step, appropriate error message or help is shown in your web application.
```

## Tools that can be used: QTP , IBM Rational , Selenium

1. Usability testing:

Usability Testing has now become a vital part of any web based project. It can be carried out by testers like you or a small focus group similar to the target audience of the web application.

2. Test the site Navigation:

Menus, buttons or Links to different pages on your site should be easily visible and consistent on all webpages

3. Test the Content:


	Content should be legible with no spelling or grammatical errors.

	Images if present should contain an "alt" text

	Tools that can be used: Chalkmark, Clicktale, Clixpy and Feedback Army


4. Interface Testing:

Three areas to be tested here are - Application, Web and Database Server

Application: Test requests are sent correctly to the Database and output at the client side is displayed correctly. Errors if any must be caught by the application and must be only shown to the administrator and not the end user.

Web Server: Test Web server is handling all application requests without any service denial.

Database Server: Make sure queries sent to the database give expected results.


Test system response when connection between the three layers (Application, Web and Database) cannot be established and appropriate message is shown to the end user.

Tools that can be used: AlertFox, Ranorex

5. Database Testing:

Database is one critical component of your web application and stress must be laid to test it thoroughly. Testing activities will include-
```
	Test if any errors are shown while executing queries

	Data Integrity is maintained while creating, updating or deleting data in database.

	Check response time of queries and fine tune them if necessary.

	Test data retrieved from your database is shown accurately in your web application

	Tools that can be used: QTP, Selenium

	```

6. Compatibility testing.

Compatibility tests ensures that your web application displays correctly across different devices. This would include-

Browser Compatibility Test: Same website in different browsers will display differently. You need to test if your web application is being displayed correctly across browsers, JavaScript, AJAX and authentication is working fine. You may also check for Mobile Browser Compatibility.

The rendering of web elements like buttons, text fields etc. changes with change in Operating System. Make sure your website works fine for various combination of Operating systems such as Windows, Linux, Mac and Browsers such as Firefox, Internet Explorer, Safari etc.

Tools that can be used: NetMechanic

7. Performance Testing:

This will ensure your site works under all loads. Testing activities will include but not limited to -


 ```
	Website application response times at different connection speeds

	Load test your web application to determine its behavior under normal and peak loads

	Stress test your web site to determine its break point when pushed to beyond normal loads at peak time.

	Test if a crash occurs due to peak load, how does the site recover from such an event

	Make sure optimization techniques like gzip compression, browser and server side cache enabled to reduce load times

	Tools that can be used: Loadrunner, JMeter

	```

8. Security testing:

Security Testing is vital for e-commerce website that store sensitive customer information like credit cards. Testing Activities will include -

```
Test unauthorized access to secure pages should not be permitted

Restricted files should not be downloadable without appropriate access

Check sessions are automatically killed after prolonged user inactivity

On use of SSL certificates, website should re-direct to encrypted SSL pages.

Tools that can be used: Babel Enterprise, BFBTester and CROSS

```


9. Crowd Testing:

You will select a large number of people (crowd) to execute tests which otherwise would have been executed a select group of people in the company. Crowdsourced testing is an interesting and upcoming concept and helps unravel many a unnoticed defects.

Tools that can be used: People like you and me !!!. And yes , loads of them!

This concludes almost all testing types applicable to your web application.



 

