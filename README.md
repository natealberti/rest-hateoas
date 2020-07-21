# rest-hateoas
"Hello, World" type of REST Hypermedia webservice 

Built using the Spring Guides. This was created using the HATEOAS library of APIs, which let me make things like links to other Spring controllers. In this one, I just linked back to the site itself. In the query string, you can also personalize the site by adding a name parameter. For example, on: http://localhost:8080/greeting?name=User the site will display "Hello, User!" This was created using three java files: Greeting.java used a base Java class from HATEOAS called RepresentationModel that lets you use links. GreetingController.java creates new instances of the Greeting class when /greeting is put into the query string. It also looks for the optional name parameter, which has its default value tied to "World." The RestHateoasApplication.java is really just the main() method, which uses Spring's SpringApplication.run() method to launch it. After creating and running the jar file, the server was running fine.
