
# State

The amount of places - in which state can be saved  
in a non-interactive client scenario - is more limited.

<br/>

## Cookies

The only proper state management facility  
that remains on the client side is cookies.

In this use case they cannot be utilized by the  
client itself, disregarding browser extensions.

As with normal browsing use cases, cookies  
may contain garbage data and are transient.

Cookies can be limited to a subpath,  
hiding them from their parent frames.

Frames can only see their own cookies  
and all of their parent frames cookies.

Permission to save cookies may not have  
been granted and has to be tested for.

<br/>

## Location

Technically the location each frame is connecting  
to could also be considered a form of state as the  
location is known to the server when connecting  
and can be changed by redirecting the client.

<br/>

## Styles

The server can generate styling rules that contain  
resources urls with state encoded in the url search  
parameters, which would becomes available once  
the rule becomes active and the resource is loaded.

<br/>

## Forms

The server can generate pre-populated form input  
elements that - when the form is submitted - will be  
transmitted back to the server.

Unlike cookies, native html input elements  
could modify the state contained within them.

<br/>

## Links

Generated links can encode state as url paramaters  
which will be transmitted when the link is clicked.

## HTTP Equiv

The server can generate meta tags with a `http-equiv`  
attribute set to `refresh` that redirects the current page  
to a specified url. 

This url can again contain state in it's url parameters.

<br/>
