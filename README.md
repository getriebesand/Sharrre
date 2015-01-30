Sharrre Plugin Mootools Version
===

Make your sharing widget!
Sharrre is originally a jQuery plugin that allows you to create nice widgets sharing for Facebook, Twitter, Google Plus (with PHP script) and more. This is the Mootools version
More information on [Sharrre] (http://sharrre.com/#demos)

Usage
===

  new Sharrre('sharrre',{
    share: {
      googlePlus: true,
      facebook: true,
      twitter: true
    },
    url: 'http://sharrre.com'
  });

Example
===
    
  <div id="demo1" data-title="sharrre" data-url="http://sharrre.com" ></div>
  window.addEvent('domready',function() {
    new Sharrre('demo1',{
      share: {
        googlePlus: true,
        facebook: true,
        twitter: true,
        delicious: true
      },
      buttons: {
        googlePlus: {size: 'tall'},
        facebook: {layout: 'box_count'},
        twitter: {count: 'vertical'},
        delicious: {size: 'tall'}
      },
      onHover: function(api, options){
        $(api.element).getElement('.buttons').show();      
      },
      onHide: function(api, options){
        $(api.element).getElement('.buttons').hide();
      }
    });
  });

  See example on [official website] (http://sharrre.com/#demos)
	

Dependencies
===

Mootools 1.4

Author
===
jQuery Version
- [Julien Hany](http://hany.fr)
- [Twitter (@_JulienH)](http://twitter.com/_JulienH)
- [Google+](http://plus.google.com/111637545317893682325)

Mootools Version
- [Sebastian]
