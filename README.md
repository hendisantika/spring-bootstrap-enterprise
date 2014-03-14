Spring Bootstrap Enterprise
======================

A Spring Web Application using Hibernate, Thymeleaf and Twitter Bootstrap built to use as a template for new projects. This project is still under heavy development but the master branch should be runnable. Be aware that some old legacy code is still included.

### Some Features
* 100% Java Config
* Spring Profiles for Environments (localhost, development, test, production)
* HSQLDB when running application in localhost environment
* MySQL when running application in development, test, production
* Hibernate JPA
* Hibernate Envars for entity revision auditing
* Spring Data JPA
* Spring Data Auditing for user and date auditing
* Spring Security login configured with different user types (root, developer, admin, user, anonymousUser)
* Spring Security Switch Filter configured for root users
* Java Melody for monitoring the application
* Logback with sifting user logs, access logs
* AOP Trace Logging
* Thymeleaf configured with the Layout Dialect and Dandelion Datatables
* GUI built with Twitter Bootstrap
* jQuery, Knockout, Underscore, Data Tables, Font Awesome, X-Editable, Select2 + a lot more front end technologies
* ... a lot more

### Getting Started

Run it in Jetty

```bash
mvn jetty:run
```

... or if you prefer Tomcat
```bash
mvn tomcat7:run
```

and open url http://localhost:8080/application-name in your browser

Log in with username root, developer, admin or user. No password required. By default the "localhost" spring profile and application properties will be used. Enjoy!


To load a spring profile with specific application properties simply provide the environment name as a compiler argument e.g.

```bash
mvn jetty:run -Dapplication.environment=test
```

just make sure you have started mysql server before you start jetty if you load other environments than "localhost". No need to create a database schema or tables. Hibernate will do that for you!


## License

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.