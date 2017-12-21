# Meet App

## Meet app is an app where you can see all upcoming IT Events.

### Components/pages used in this application: 

__meet-app.html__ - main application file which merges all other components in Single Page Application.
Using [iron-pages](https://www.webcomponents.org/element/PolymerElements/iron-pages) to create site pages and [App-Route](https://www.webcomponents.org/element/PolymerElements/app-route) to navigate between iron-pages.

__meet-home.html__ - home page component, you can see this component on the main '/' page. Creates big slider using [skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) component.

__meet-events.html__ - home page component, you can see this component on the main '/' page. Creates a list of items(upcoming events) using [dom-repeat](https://www.polymer-project.org/2.0/docs/api/elements/Polymer.DomRepeat).
Number of items based on Polymer Object which contains data.

__meet-google.html/meet-facebook.html__ - events pages with some info about events and link for Register.

__meet-registration.html__ - registration page with __meet-regfield.html__ component that creates registration field

__meet-404-warning.html__ - 404 Page, you can see this page every time you follow incorrect url.

__meet-button.html__ - button component, creates stylized button, used in __meet-home.html__ , __meet-google.html/meet-facebook.html__

__meet-regfield.html__ - Registration field component, creates stylized & configured registration field with POST method that send data to the [server](https://httpbin.org), used in __meet-registration.html__
Component using [paper-input](https://www.webcomponents.org/element/PolymerElements/paper-input), [iron-form](https://www.webcomponents.org/element/PolymerElements/iron-form), [paper-checkbox](https://www.webcomponents.org/element/PolymerElements/paper-checkbox) and
[paper-button](https://www.webcomponents.org/element/PolymerElements/paper-button) components for registration form.




Third party components used:
[skeleton-carousel](https://www.webcomponents.org/element/FabricElements/skeleton-carousel) -  web component that provides a carousel for images and other content.
(used on home page)
