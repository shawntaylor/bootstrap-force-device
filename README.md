bootstrap-force-device
======================

Simulate a different device width within a given bootstrap container.

DEMO: http://shawntaylor.github.io/bootstrap-force-device/

Only requires CSS. Just add the .force-device CSS into your project AFTER the Bootstrap CSS, and add .force-xs, .force-sm, .force-md or .force-lg to any div containing the content you want to force to behave like it's on a different device. That's it.

The most common use case for this is if you want to have the same content within a modal as you do elsewhere in your site, and don't want to write the content twice to account for the smaller width of the modal. In this case, best place to put the .force-* class is on the .modal-body.
Like so:
----
    <div class="modal-body force-xs">
      <div class="col-md-6 col-xs-8">Some stuff</div>
      <div class="col-md-6 col-xs-4">Other stuff</div>
    </div>
