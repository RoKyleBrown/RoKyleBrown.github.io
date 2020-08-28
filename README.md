## Portfolio Site

[Live Link](https://rokylebrown.github.io/)

![alt text](https://ballup-dev.s3-us-west-1.amazonaws.com/Screen+Shot+2020-08-26+at+9.58.58+AM.png "ScreenShot1")

### Overview

This site was built with Vanilla JavaScript, jQuery, HTML5, and CSS3. The preload animation was made in Adobe After Effects. The page hosts my mission statement, skills, projects, and contact info. 

![alt text](https://ballup-dev.s3-us-west-1.amazonaws.com/Screen+Shot+2020-08-28+at+3.37.41+AM.png "ScreenShot2")

### Functionality

Checks to see if the "Skills" module is visable on the browser and is 70% in view. Once this is true, the source image is changed to a pixelized version so that the overlaying content is more prominent. You will see the effect if you focus on the ones and zeros in the background. 

```javascript
        function isInViewport(element) {
            let el = document.getElementById(element);

            let hero2 = el.getBoundingClientRect();
            if ((hero2.bottom - (hero2.height*.3)) <= (window.innerHeight || 
            document.documentElement.clientHeight)){
                el.src = "hero2-3.jpg";
            } else {
                el.src = "hero2-0.jpg"
            }
        }
```

![alt text](https://ballup-dev.s3-us-west-1.amazonaws.com/Screen+Shot+2020-08-28+at+3.38.20+AM.png "ScreenShot3")
