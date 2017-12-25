# Meet App

## Meet app is an app where you can see all upcoming IT Events.

### App structure
The main page (https://arestch.github.io/) contains header(created using [app-layout](https://www.webcomponents.org/element/PolymerElements/app-layout)), big slider section (__meet-home.html__) and list of upcoming events(__meet-events.html__).
You can navigate to the event page with button in the slider\on the event image in the "UPCOMING EVENTS" section.
Event page (/google or /facebook) contains some information about event and button leading to the registration page.
Registration page contains registration form. The ​registration ​form data submitted to a httbin.org using POST method.


### Components/pages belonging to this application: 

__meet-app.html__ - main application file which merges all other components in Single Page Application.
Using [iron-pages](https://www.webcomponents.org/element/PolymerElements/iron-pages) to create site pages and [App-Route](https://www.webcomponents.org/element/PolymerElements/app-route) to navigate between iron-pages.

__meet-home.html__ - home page component, you can see this component on the main '/' page. Creates big slider using [skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) component.

__meet-events.html__ - home page component, you can see this component on the main '/' page. Creates a list of items(upcoming events) using [dom-repeat](https://www.polymer-project.org/2.0/docs/api/elements/Polymer.DomRepeat).
Number of items based on Polymer Object which contains data.

__meet-google.html/meet-facebook.html__ - events pages with some info about events and link for Register.

__meet-registration.html__ - registration page with __meet-regfield.html__ component that creates registration field

__meet-404-warning.html__ - 404 Page, you can see this page every time you follow incorrect url.

__meet-button.html__ - button component, creates stylized button, used in __meet-home.html__ __meet-google.html/meet-facebook.html__

__meet-regfield.html__ - Registration field component, creates stylized & configured registration field with POST method that send data to the [server](https://httpbin.org), used in __meet-registration.html__
Component using [paper-input](https://www.webcomponents.org/element/PolymerElements/paper-input), [iron-form](https://www.webcomponents.org/element/PolymerElements/iron-form), [paper-checkbox](https://www.webcomponents.org/element/PolymerElements/paper-checkbox) and
[paper-button](https://www.webcomponents.org/element/PolymerElements/paper-button) components for registration form.

### Technologies used:
[dom-repeat](https://www.polymer-project.org/2.0/docs/api/elements/Polymer.DomRepeat) - used in __meet-events__ for creating a list of upcoming events(items). Items is taken from the built-in object but it can be moved in json file aswell.

### WebComponents used in this application:
[App-Route](https://www.webcomponents.org/element/PolymerElements/app-route) - used for navigation between pages in __meet-app.html__ 

[iron-pages](https://www.webcomponents.org/element/PolymerElements/iron-pages) - used for navigation between pages in __meet-app.html__

[paper-input](https://www.webcomponents.org/element/PolymerElements/paper-input) - used for registration form in __meet-regfield.html__

[paper-checkbox](https://www.webcomponents.org/element/PolymerElements/paper-checkbox) - used for registration form in __meet-regfield.html__

[paper-button](https://www.webcomponents.org/element/PolymerElements/paper-button) - used for registration form in __meet-regfield.html__

[iron-form](https://www.webcomponents.org/element/PolymerElements/iron-form) - used for registration form in __meet-regfield.html__

[iron-icon](https://www.webcomponents.org/element/PolymerElements/iron-icon) - used to create icons.

[skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) - used for slider in __meet-home.html__

[paper-icon-button](https://www.webcomponents.org/element/PolymerElements/paper-icon-button) - [skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) dependency.

[iron-icons](https://www.webcomponents.org/element/PolymerElements/iron-icons/elements/iron-icons)  - [skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) dependency & need for [iron-icon](https://www.webcomponents.org/element/PolymerElements/iron-icon).