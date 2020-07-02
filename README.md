# SpringMavenWebApp
This projects also configures the application.
For dev configuration add the properties to application-dev.properties in src/main/resources
For production configuration add the properties to application-prod.properties in src/main/resources
For common configurations, add configurations in application.properties in src/main/resources
To activate a particular profile(config) give the following command in the command line : -Dspring-boot.run.profiles={profileName}
example: mvnw spring-boot:run -Dspring-boot.run.profiles=dev
