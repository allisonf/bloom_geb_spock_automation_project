Replace the dummy tests with your actual spock test code in the specs folder.
Put the Geb pages in a pages directory at the same level as the specs directory.
The rest of the project is the gradle setup. Gradle is the build tool and nothing needs to be done with that.

The following commands will launch the tests with the individual browsers:

    ./gradlew chromeTest
    ./gradlew firefoxTest

    or

    ./gradlew test
    to run the tests in all browsers

    Replace ./gradlew with gradlew.bat if you are running the examples in Windows.

Note: Due to a bug in Firefox 32.0, you must downgrade to Firefox 30 for firefoxTest to pass.

The first time you run these tests, a lot of stuff will be download. It will take a couple minutes.

Test results may be found in: build/reports/firefoxTest/tests/index.html
Output can be seen by clicking the Standard Output link once you've clicked into the output for a particular test class.
