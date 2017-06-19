### Status
[![Build Status](https://travis-ci.org/astrashevskiy/MobileQA.png)](https://travis-ci.org/astrashevskiy/MobileQA)

## [Documentation](https://astrashevskiy.github.io/MobileQA/)

## [Test Plan](TestPlan.md)


execute tests with
"mvn test" - this will execute tests using SauceLabs device farm (one need to set environment variables SAUCE_USER and SAUCE_KEY with values from one's SauceLab account). To run test locally one need to comment/uncomment app property in [capabilities.properties](src/test/resources/capabilities.properties) and run "mvn -Dorg.no.run.local=true test".

and then to generate allure use
"mvn site"

or all-together
"mvn clean test site"
