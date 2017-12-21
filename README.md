# Meet App

## Meet app is an app where you can see all upcoming IT Events.

### Components\pages used in this application: 

__meet-app.html__ - main application file which merges all other components in Single Page Application.
Using [iron-pages](https://www.webcomponents.org/element/PolymerElements/iron-pages) to create site pages and [App-Route](https://www.webcomponents.org/element/PolymerElements/app-route) to navigate between iron-pages.

__meet-home.html__ - home page component, you can see this component on the main '/' page. Creates big slider using [skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) component.

__meet-events.html__ - home page component, you can see this component on the main '/' page. Creates a list of items(upcoming events) using [dom-repeat](https://www.polymer-project.org/2.0/docs/api/elements/Polymer.DomRepeat).
Number of items based on Polymer Object which contains data.

__meet-google.html/meet-facebook.html__ - events pages with some info about events and link for Register.

__meet-registration.html__ - page with registration form with HTTP POST method that sends data to the [server](https://httpbin.org).

__meet-404-warning.html__ - 404 Page, you can see this page every time you follow incorrect url.

__meet-button.html__ - button component, creates stylized button, used in __meet-home.html__ , __meet-google.html/meet-facebook.html__ 



Third party components used:
[skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) -  web component that provides a carousel for images and other content.
(used on home page)
