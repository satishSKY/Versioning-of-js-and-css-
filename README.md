# Versioning-of-js-and-css-

Give dynamic versioning for css and js files by using javascript.  




var jsVersion = parseInt(Math.random()*1000000000);
    var script = document.getElementsByTagName('script');
    var link = document.getElementsByTagName('link');
     for (var int = 0; int < link.length; int++) { 
        link[int].href = link[int].href + "?ver=" + jsVersion;
        console.log(link[int].href);
    }   
    for (var int = 0; int < script.length; int++) { 
        script[int].src = script[int].src + "?ver=" + jsVersion;
        console.log(script[int].src);
    }    
