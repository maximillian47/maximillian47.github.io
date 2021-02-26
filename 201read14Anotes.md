# Some cool CSS transitions
  * fade in 
  ```css
      .fade 
      { 
        opacity: 0.5;
      }
      .fade:hover
      {
        opacity:1;
      }
  ```
  * change color
  ```css
      .color:hover
      {
        background:#53a7ea;
      }
  ```
  * grow & shrink
  ```css
      .grow:hover
      {
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
      }
  ```
  * rotate elements
  ```css
     .rotate:hover
      {
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
      }
  ```
  * square to circle 
  ```css
      .circle:hover
      {
        border-radius: 50%;
      }
  ```
  * 3d shadow 
  ```css
      .threed:hover 
      { 
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
      }
  ```
  * swing
  ```css
      @-webkit-keyframes swing
      { 
          15%
          {
              -webkit-transform: translateX(5px);
              transform: translateX(5px);
          }
          30%
          {
              -webkit-transform: translateX(-5px);
              transform: translateX(-5px);
          }
          50%
          {
              -webkit-transform: translateX(3px);
              transform: translateX(3px);
          }
          65%
          {
              -webkit-transform: translateX(-3px);
              transform: translateX(-3px);
          }
          80%
          {
              -webkit-transform: translateX(2px);
              transform: translateX(2px);
          }
          100%
          {
              -webkit-transform: translateX(0);
              transform: translateX(0);
          }
      }
            
      @keyframes swing
      { 
          15%
          {
              -webkit-transform: translateX(5px);
              transform: translateX(5px);
          }
          30%
          {
              -webkit-transform: translateX(-5px);
              transform: translateX(-5px);
          }
          50%
          {
              -webkit-transform: translateX(3px);
              transform: translateX(3px);
          }
          65%
          {
              -webkit-transform: translateX(-3px);
              transform: translateX(-3px);
          }
          80%
          {
              -webkit-transform: translateX(2px);
              transform: translateX(2px);
          }
          100%
          {
              -webkit-transform: translateX(0);
              transform: translateX(0);
          }
      }
      
      .swing:hover
      {
              -webkit-animation: swing 1s ease;
              animation: swing 1s ease;
              -webkit-animation-iteration-count: 1;
              animation-iteration-count: 1;
      }
      
  ``` 
  * inset border
  ```css
      .border:hover
      {
              box-shadow: inset 0 0 0 25px #53a7ea;
      }
  ```
