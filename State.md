
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

<br/>

## Location

Technically the location each frame is connecting  
to could also be considered a form of state as the  
location is known to the server when connecting  
and can be changed by redirecting the client.

