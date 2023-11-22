# findYourJobScript
Script to find an specific job in a collections of websites

## **How to Work**<br />
* Import collection and environment to postman <br />
* Once both files are imported, click on *training* collection <br />
* Click on Run button
* Click on *Select File* 
* Select the **data.cvs** file
* Click on *Run training*

There is another way to execute
* Open your terminal
* Go to the project
* Run this command: <br />
`newman run training.postman_collection.json --reporter-htmlextra-export report-api_TestReport.html --environment=finding.postman_environment.json -d data.csv -r cli,htmlextra`


## **How to find an specific job**<br />
* Open the *finding* environment
* Edit the *jobs* variable (if you want to search for more than one, separate the words with comma)

## **How to Check the results**<br />
There are two ways to check results:

1. Checking logs in the console (A message will displayed: "HAY ALGÚN PUESTO VACANTE EN `{company}`".
2. Viewing the Run Summary section, All tests passed mean that there is a job available.
