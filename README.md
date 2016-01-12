# phantomjs2-helpers
PhantomJS2 helpers and hooks

get-local-image
```
var ImageDataResolver = require('helpers/get-local-image/getLocalImage.js');

// ordered Array of images with paths, callback

ImageDataResolver(['./img_g.png','./img_r.png'],function(result){
	 console.log(result);
	 ==> ['data:image/png;base64,...{img_g.png}','data:image/png;base64,...{img_r.png}']
});
```
> 
This hook for PhantomCSS && Phantomjs 2.0.0-2.0.1 compability
because "casper.fillSelectors" does not working for input[type="file"] in this Phantomjs versions
PhantomCSS.initClient..->run should be rewrited with this idea
