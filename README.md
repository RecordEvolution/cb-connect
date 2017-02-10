##&lt;cb-connect&gt;


`cb-connect` is an element which connects to a [crossbar.io](http://crossbar.io) router.
Simply add the `cb-connect` element to your index.html or custom element. As soon as the connection is established, `cb-connect` will fire an event, which contains the session details, to the target element.

Example:

<!---
```
    <cb-connect target-element="main-page"></cb-connect>
    <main-page></main-page> 
```
-->
