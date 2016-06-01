# react.waves
React Implementation of the animated wave codpen here:
https://codepen.io/loktar00/pen/kfrKC

##Usage

###JS
```javascript
import Waves from 'react.waves'

...

<Waves></Waves>
```

###CSS
Apply the following CSS:
```css

#ocean{
  overflow: hidden;
  position:relative;
  display: flex;
  width:100%;
  height:100%;
  background-image: -webkit-gradient(
  linear,
  left bottom,
  left top,
  color-stop(0, rgb(255,255,255)),
  color-stop(0.50, rgb(0,150,255))
  );
}

.wave{
  background:#a8e3ff;
  display:flex;
  height:60%;
  width:10px;
  position:absolute;
  -webkit-animation-name:             WaveKeyframe;
  -webkit-animation-duration:         10s;
  -webkit-animation-iteration-count:  infinite;
  -webkit-transition-timing-function: ease-in-out;
}

@-webkit-keyframes WaveKeyframe{
  0%{
    height:60%;
  }
  50%{
    height:40%;
  }
  100%{
    height:60%;
  }
}
```
