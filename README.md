
### Environment Setup

1. Global Dependencies
    * [Install Maven](https://maven.apache.org/install.html)
    * Or Install Maven with [Homebrew](http://brew.sh/)
    ```
    $ brew install maven
    ```
2. Sauce Credentials
    * In the terminal export your Sauce Labs Credentials as environmental variables:
    ```
    $ export SAUCE_USERNAME=<your Sauce Labs username>
	$ export SAUCE_ACCESS_KEY=<your Sauce Labs access key>
    ```
3. Project Dependencies
	* Check that Packages are available
	```
	$ cd Java-TestNg-Selenium
	$ mvn test-compile
	```
	* You may also want to run the command below to check for outdated dependencies. Please be sure to verify and review updates before editing your pom.xml file. The updated packages may or may not be compatible with your code.
	```
	$ mvn versions:display-dependency-updates
	```
### Running Tests

Tests in Parallel:
	
	Example: 
	$ mvn -X clean test -DsuiteFile=parameterexample100VMS.xml
	
	NOTE you can use any file in the repo.
