# ipt-angular2-reactive-websocket-demo
End-to-end reactive WebSockets demo with Angular 2 (TypeScript) and RxJS (RxNext) and JavaSE + Project Reactor at server side. No web server needed - all resources as well as live WebSocket events are served by custom reactive HTTP endpoint using Reactor Net.

Custom reactive IPTRxWebSocketSubject component implemented exposing WebSocket as RxJS buidirectional subject (by idea from RxDOM), plus reactive WebSocket open and close observers.

The presentation accompanying this demo is available at:
http://www.slideshare.net/Trayan_Iliev/ipt-high-performance-reactive-programming-with-java-8-and-javascript

Limitaion: Demo works well in Chrome, but not in Firefox, because of WebSocket implementation coming from Reactor Net. Further investigation needed.

