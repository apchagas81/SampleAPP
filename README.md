# ACME

## Overview

[Include a brief overview of the project here.]

## Testing and Code Scanning Documentation

| Aspect              | Frontend (Angular)                                                                   | Backend (Java)                                                                     |
|---------------------|--------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| **Testing Framework** | Jest                                                                                 | JUnit                                                                              |
| **Unit Testing**     | - Run tests with `npm test`<br>- Write tests in `src/app`<br>- Coverage: Jest built-in | - Run tests with `mvn test`<br>- Write tests in `src/test/java`<br>- Coverage: JaCoCo |
| **Integration Testing** | - Run tests with `npm test`<br>- Write tests in `src/app`<br>- Coverage: Jest built-in | - Run tests with `mvn test`<br>- Write tests in `src/test/java`<br>- Coverage: JaCoCo |
| **Exporting Results to SonarQube** | Execute `sonar-scanner` after running tests                             | Execute `mvn sonar:sonar` after running tests                                     |

## Installation

[Include installation instructions here.]

## Usage

[Include usage instructions here.]

## Contributing

[Include contributing guidelines here.]

## License

[Include license information here.]

## Testing Instructions

### Frontend (Angular Application)

#### Unit Testing with Jest

##### Overview

Unit testing is performed using the Jest framework. Jest is a delightful JavaScript testing framework with a focus on simplicity.

##### Instructions

1. **Running Unit Tests Locally:**
   - Navigate to the Angular application directory.
   - Run the following command:
     ```bash
     npm test
     ```
   - This command will execute all unit tests and display the results in the console.

2. **Writing Unit Tests:**
   - Unit tests are located in the `src/app` directory, alongside the components and services they are testing.
   - Each test file should have a `.spec.ts` extension.
   - Use Jest's testing utilities and matchers to write descriptive and accurate tests.

3. **Test Coverage:**
   - Jest provides built-in coverage reporting.
   - After running tests, a coverage report will be generated in the `coverage` directory.
   - Review the report to ensure adequate test coverage.

4. **Exporting Results to SonarQube:**
   - Configure SonarQube in your project's CI/CD pipeline.
   - After running unit tests, execute the following command to export test results to SonarQube:
     ```bash
     sonar-scanner
     ```

### Backend (Java Application)

#### Unit Testing with JUnit

##### Overview

Unit testing in the Java application is performed using the JUnit framework. JUnit is a simple framework to write repeatable tests.

##### Instructions

1. **Running Unit Tests Locally:**
   - Navigate to the Java application directory.
   - Run the following command to execute unit tests:
     ```bash
     mvn test
     ```
   - This command will run all unit tests and display the results in the console.

2. **Writing Unit Tests:**
   - Unit tests are located in the `src/test/java` directory, separate from production code.
   - Each test class should have a corresponding class in the `src/main/java` directory.
   - Use JUnit annotations and assertions to write effective tests.

3. **Test Coverage:**
   - Test coverage is measured using JaCoCo, a code coverage library.
   - After running tests, a coverage report will be generated in the `target/site/jacoco` directory.
   - Open the HTML report in a browser to view code coverage statistics.

4. **Exporting Results to SonarQube:**
   - Configure SonarQube in your project's CI/CD pipeline.
   - After running unit tests, execute the following command to export test results to SonarQube:
     ```bash
     mvn sonar:sonar
     ```

You can copy and paste this Markdown content into your README.md file. Feel free to customize the sections as needed! Let me know if you need any further assistance!
