## Testing Documentation

| Aspect              | Frontend (Angular)                                                                   | Backend (Java)                                                                     |
|---------------------|--------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
| **Testing Framework** | Jest                                                                                 | JUnit                                                                              |
| **Unit Testing**     | - Run tests with `npm test`<br>- Write tests in `src/app`<br>- Coverage: Jest built-in | - Run tests with `mvn test`<br>- Write tests in `src/test/java`<br>- Coverage: JaCoCo |
| **Integration Testing** | Not applicable                                                             | Not applicable                                                                     |
| **Exporting Results to SonarQube** | Execute `sonar-scanner` after running tests                             | Execute `mvn sonar:sonar` after running tests                                     |
