# Script for Angular Spring Boot Spring Tip

* look at the concerns front-end developers (use Angular + TypeScript) face when talking to Spring Boot services (use Kotlin)
 * REST client
 * CORS
 * WebSockets


* create a simple REST API with `Customer` data using Reactive Spring MVC  and a Reactive MongoDB repository. NB: we're using `Publisher<Customer ` on the backend
* create an angular app using `ng new client`. create a `@Injectable()` `CustomerService` provider that returns the `Customer` data from the service. NB: it'll use RxJS and observables on the client usign the `Http` object
* oops! Doesn't work. Add `@CrossOrigin (hosts= "*")` to make that work.
* we need to notify the client when new data gets added. We can use eiher SSE or WebSockets. See [this link](https://docs.spring.io/spring-framework/docs/5.0.0.RC1/spring-framework-reference/web.html#web-reactive-websocket-support) for more.
* 
