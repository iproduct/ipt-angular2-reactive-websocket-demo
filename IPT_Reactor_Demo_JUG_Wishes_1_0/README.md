# IPT Reactor Demo: JUG Wishes 1.0
End-to-end reactive WebSockets demo with Angular 2 (TypeScript) and RxJS (RxNext) and JavaSE + Project Reactor at server side. No web server needed - all resources as well as live WebSocket events are served by custom reactive HTTP endpoint using Reactor Net.

JavaScript (TypeScript) client part is available in src/main/webapp folder. The main application component class AppComponent is in src/main/webapp/app folder, together with custom reactive WebSocket implementation - IPTRxWebSocketSubject component. IPTRxWebSocketSubject is exposing WebSocket as RxJS bidirectional subject (by idea from RxDOM), plus reactive WebSocket open and close observers.

Server side is implemented using Reactor (http://projectreactor.io/) project. Main main class is reactor.ReactorWishesWS in src/main/java folder. It serves all resources required by the client using Reactor Net (Netty), and could be started as console application - no webserver required. It also implements reactive WebSocket endpoint (see wsHandler() method).

The presentation accompanying this demo is available at: http://www.slideshare.net/Trayan_Iliev/ipt-high-performance-reactive-programming-with-java-8-and-javascript

Limitaion: Demo works well in Chrome, but not in Firefox, because of WebSocket implementation coming from Reactor Net. Further investigation needed.
