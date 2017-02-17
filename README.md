##&lt;cb-connect&gt;


`cb-connect` is an element which connects to a [crossbar.io](http://crossbar.io) router.
Simply add the `cb-connect` element to the local DOM of your custom element. As soon as the connection is established, `cb-connect` will fire an event, which contains the session details.

Example:


```html
<dom-module id="custom-element">
  <template>
    <cb-connect on-crossbar-connected="eventHandler"></cb-connect>
  </template>

  <script>
    Polymer({

      properties: {

      },

      eventHandler: function(e) {
        console.log('connected, the session object is:', e.detail);
      }

    });
  </script>
</dom-module>
```
Instead of listening to the event, you could also add an observer for the session object.

