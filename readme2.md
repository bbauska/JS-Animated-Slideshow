<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- 1. Anime.js -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<h2>1. Anime js  https://animejs.com/</h2>

<p>As a Javascript animation library, <a href="https://github.com/juliangarnier/anime">Anime.js</a> provides a simple yet powerful API that allows work to be done quickly.</p>

<p>It can work with CSS properties, SVG files, DOM attributes, and JavaScript objects. The animations can be played, paused, restarted, reversed, or stopped with the help of Anime.js. Apart from these features, the library also provides a phenomenal number of features for animating elements with follow-throughs and overlaps. Also, we can listen to animation-related events using callbacks and promises, which allow us to get notified whenever we see something that is animated.</p>

<p>One of the key benefits of <a href="https://github.com/juliangarnier/anime">Anime.js</a> is its flexibility. The library allows users to create a wide range of animations, from simple motion to complex and multi-layered effects. This makes it well-suited for various animation needs, from simple UI animations to more elaborate and interactive effects.</p>

<p>Another advantage of Anime.js is its ease of use. The library has a simple and intuitive API that makes it easy for developers to get started with the library and create their first animations. Even if you’re new to web animation, you can quickly and easily create smooth and engaging animations with Anime.js.</p>

<p>An animation library like Anime.js is undoubtedly one of the best on the market. From their website landing page, you can feel the power it offers with the beautiful animations it is built on.</p>

<p>Below are some examples of animation made with anime.js</p>

<p>Morphing: Creates transition between two SVG shapes.</p>

```
<!-- html -->

  <script src="https://cdn.jsdelivr.net/npm/animejs@3.0.1/lib/anime.min.js"></script>


<svg id="demo-svg" width="600" height="600">
    <polygon stroke="none" fill="gray"
        points=" 400 150 , 300 250 , 300 400 , 400 500 , 500 400 , 500 250 , 400 150">
    </polygon>
</svg>

<!-- css -->
<style>
    body{
  background-image: linear-gradient(to right, rgb(242, 112, 156), rgb(255, 148, 114));
}
#demo-svg path{
    stroke-dasharray: 1000;
    stroke-dashoffset: 0;
</style>
```

```
 // anime.js

anime({
    targets: '#demo-svg polygon',
    points: [
        { value: '400 150 , 300 250 , 300 400 , 400 500 , 500 400 , 500 250 , 400 150'},
        { value: '400 200 , 400 350 , 300 450 , 400 350 , 500 450 , 400 350 , 400 200'}
    ],
    easing: 'easeOutQuad',
    duration: 2500,
    loop: true
});
```

<P>Line Drawing: Creates path drawing animation using the 'stroke-dashoffset' property. Set the path “dash-offset” value with anime.setDashoffset() in a from to formatted value.</p>

<p>image03 for anime.js</p>

```
<!-- html -->

  <script src="https://cdn.jsdelivr.net/npm/animejs@3.0.1/lib/anime.min.js"></script>

<svg id="demo"  width="1385px" height="256px">
        <path stroke="blue" stroke-width="3" fill="url(#PSgrad_0)" d="M1348.721,156.648 C1331.497,202.034 1319.740,225.274 1303.335,239.491 C1291.579,249.881 1279.822,253.982 1273.807,255.075 L1267.792,234.843 C1273.807,232.929 1281.736,229.101 1288.845,223.086 C1295.407,217.892 1303.609,208.596 1309.077,196.292 C1310.171,193.832 1310.991,191.918 1310.991,190.551 C1310.991,189.184 1310.444,187.270 1309.350,184.262 L1260.410,62.322 L1286.657,62.322 L1315.639,140.517 C1318.646,149.266 1321.927,159.655 1324.115,167.584 L1324.661,167.584 C1327.122,159.655 1329.856,149.539 1333.137,139.970 L1359.384,62.322 L1384.812,62.322 L1348.721,156.648 ZM1219.680,177.974 L1218.860,177.974 C1211.478,188.363 1197.260,197.659 1178.395,197.659 C1151.601,197.659 1137.931,178.794 1137.931,159.655 C1137.931,127.666 1166.365,110.168 1217.493,110.442 L1217.493,107.708 C1217.493,96.771 1214.485,77.086 1187.418,77.086 C1175.114,77.086 1162.264,80.913 1152.968,86.928 L1147.500,71.071 C1158.436,63.962 1174.294,59.314 1190.972,59.314 C1231.437,59.314 1241.279,86.928 1241.279,113.449 L1241.279,162.936 C1241.279,174.419 1241.826,185.629 1243.467,194.652 L1221.594,194.652 L1219.680,177.974 ZM1218.040,127.120 C1191.792,126.573 1161.991,131.221 1161.991,156.921 C1161.991,172.506 1172.380,179.888 1184.684,179.888 C1201.908,179.888 1212.845,168.951 1216.673,157.741 C1217.493,155.281 1218.040,152.547 1218.040,150.086 L1218.040,127.120 ZM1083.799,0.531 L1107.859,0.531 L1107.859,194.652 L1083.799,194.652 L1083.799,0.531 ZM993.310,197.659 C975.812,197.659 960.501,190.004 952.572,176.880 L952.026,176.880 L952.026,248.787 L928.239,248.787 L928.239,105.520 C928.239,88.569 927.692,74.898 927.145,62.322 L948.745,62.322 L949.838,85.015 L950.385,85.015 C960.228,68.883 975.812,59.314 997.412,59.314 C1029.400,59.314 1053.460,86.382 1053.460,126.573 C1053.460,174.146 1024.479,197.659 993.310,197.659 ZM990.029,78.453 C973.625,78.453 958.314,90.209 953.666,108.254 C952.846,111.262 952.026,114.816 952.026,118.097 L952.026,140.790 C952.026,144.344 952.572,147.625 953.119,150.633 C957.494,167.311 971.984,178.794 989.209,178.794 C1014.636,178.794 1029.400,158.015 1029.400,127.666 C1029.400,101.146 1015.457,78.453 990.029,78.453 ZM804.666,132.861 C805.213,165.397 825.992,178.794 850.052,178.794 C867.277,178.794 877.666,175.787 886.689,171.959 L890.790,189.184 C882.314,193.011 867.824,197.386 846.771,197.386 C806.033,197.386 781.700,170.592 781.700,130.674 C781.700,90.756 805.213,59.314 843.764,59.314 C886.962,59.314 898.446,97.318 898.446,121.651 C898.446,126.573 897.899,130.401 897.625,132.861 L804.666,132.861 ZM841.850,76.539 C817.516,76.539 806.853,98.958 804.940,115.636 L875.206,115.636 C875.479,100.325 868.917,76.539 841.850,76.539 ZM749.720,144.071 C755.735,169.772 760.109,187.543 763.937,194.652 L739.330,194.652 C736.323,189.457 732.222,173.599 727.027,150.633 C721.559,125.206 711.716,115.636 690.117,114.816 L667.697,114.816 L667.697,194.652 L643.910,194.652 L643.910,12.834 C655.940,10.374 673.165,9.007 689.570,9.007 C714.997,9.007 731.401,13.655 742.885,24.044 C752.181,32.246 757.375,44.823 757.375,59.041 C757.375,83.374 742.064,99.505 722.652,106.067 L722.652,106.887 C736.870,111.809 745.345,124.932 749.720,144.071 ZM733.589,61.775 C733.589,37.988 716.364,27.599 691.210,27.325 C679.727,27.325 671.525,28.419 667.697,29.512 L667.697,96.771 L692.030,96.771 C717.457,96.771 733.589,82.827 733.589,61.775 ZM579.942,118.371 C579.942,97.045 572.013,79.273 549.320,79.273 C533.462,79.273 521.159,90.483 517.058,103.880 C515.964,106.887 515.417,110.988 515.417,115.090 L515.417,194.652 L491.357,194.652 L491.357,98.138 C491.357,84.468 491.084,73.258 490.263,62.322 L511.589,62.322 L512.956,84.194 L513.503,84.194 C520.065,71.617 535.376,59.314 557.249,59.314 C575.567,59.314 604.002,70.250 604.002,115.636 L604.002,194.652 L579.942,194.652 L579.942,118.371 ZM367.784,132.861 C368.331,165.397 389.110,178.794 413.170,178.794 C430.395,178.794 440.785,175.787 449.807,171.959 L453.908,189.184 C445.433,193.011 430.942,197.386 409.889,197.386 C369.151,197.386 344.818,170.592 344.818,130.674 C344.818,90.756 368.331,59.314 406.882,59.314 C450.081,59.314 461.564,97.318 461.564,121.651 C461.564,126.573 461.017,130.401 460.744,132.861 L367.784,132.861 ZM404.968,76.539 C380.634,76.539 369.972,98.958 368.058,115.636 L438.324,115.636 C438.597,100.325 432.035,76.539 404.968,76.539 ZM263.898,197.659 C246.400,197.659 231.089,190.004 223.160,176.880 L222.613,176.880 L222.613,248.787 L198.827,248.787 L198.827,105.520 C198.827,88.569 198.280,74.898 197.733,62.322 L219.332,62.322 L220.426,85.015 L220.973,85.015 C230.816,68.883 246.400,59.314 267.999,59.314 C299.988,59.314 324.048,86.382 324.048,126.573 C324.048,174.146 295.067,197.659 263.898,197.659 ZM260.617,78.453 C244.213,78.453 228.902,90.209 224.254,108.254 C223.433,111.262 222.613,114.816 222.613,118.097 L222.613,140.790 C222.613,144.344 223.160,147.625 223.707,150.633 C228.081,167.311 242.572,178.794 259.797,178.794 C285.224,178.794 299.988,158.015 299.988,127.666 C299.988,101.146 286.044,78.453 260.617,78.453 ZM83.186,197.659 C34.519,197.659 0.343,159.929 0.343,104.153 C0.343,45.644 36.706,7.366 85.920,7.366 C136.227,7.366 168.763,45.917 168.763,100.599 C168.763,164.030 130.212,197.659 83.186,197.659 ZM84.826,26.778 C45.455,26.778 25.770,63.142 25.770,103.606 C25.770,142.977 47.096,178.247 84.553,178.247 C122.283,178.247 143.609,143.524 143.609,101.693 C143.609,65.056 124.471,26.778 84.826,26.778 Z" />
    </svg>
```
```
 // anime.js

anime({
  targets: '#demo path',
  strokeDashoffset: [anime.setDashoffset, 0],
  easing: 'easeInOutQuad',
  duration: 7500,
  delay: function(el, i) { return i * 250 },
  direction: 'alternate',
  loop: true
});
```

<p>These are basic examples, but Anime.js offers many more options and features for creating complex 
and sophisticated animations. You can learn more about using Anime.js by reading the documentation 
and tutorials on the Anime.js website.</p>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- 2. three.js -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<a href="https://threejs.org/">Three.js</a>

<h2>2. Three js  https://threejs.com/</h2>

<p>Three.js is a web-based cross-browser JavaScript library and application programming interface 
which allows the creation of 3D animations for computer graphics in a web browser of any platform 
by utilizing WebGL and a JavaScript library and application programming interface called Three.js.</p>

<p>The Three.js framework has been designed to make creating 3D computer animations that display in 
the browser easier, without the need for a standalone application or a plugin, as in traditional cases.</p>

<p>One of the key benefits of Three.js is its versatility. The library allows developers to create a 
wide range of 3D graphics and animations, from simple geometric shapes to complex and detailed models. 
This makes it well-suited for a variety of applications, from games and interactive experiences to 
data visualizations and augmented reality.</p>

<p>Another advantage of Three.js is its performance. Because it is built on top of WebGL, it can use the 
GPU on users’ devices to create high-performance graphics and animations. This means users can experience 
smooth and responsive graphics and animations, even on devices with limited resources.</p>

<p>Below are some examples of animation made with Three.js</p>

```
 // three.js

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r120/three.min.js"></script>

// create scene
var scene = new THREE.Scene();

// create camera
var camera = new THREE.PerspectiveCamera( 75, window.innerWidth / window.innerHeight, 0.1, 1000 );

// create renderer
var renderer = new THREE.WebGLRenderer();
renderer.setSize( window.innerWidth, window.innerHeight );

// add the renderer to the page
document.body.appendChild( renderer.domElement );

// create cube
var geometry = new THREE.BoxGeometry( 1, 1, 1 );
var material = new THREE.MeshBasicMaterial( { color: 0x808080} );
var cube = new THREE.Mesh( geometry, material );

// add cube to scene
scene.add( cube );

// move  camera back
camera.position.z = 5;

// animate
function animate() {
  requestAnimationFrame( animate );
  cube.rotation.x += 0.01;
  cube.rotation.y += 0.01;
  renderer.render( scene, camera );
}
animate();
```

<p>This is an elementary example, but it shows the basic steps involved in creating a 3D scene with 
Three.js. You can learn more about using Three.js by reading the documentation and tutorials on the 
Three.js website.</p>

<p>Overall, Three.js is a powerful and versatile library for creating 3D graphics and animations on 
the web. Whether you’re a web developer looking to create immersive experiences or a designer looking 
to visualize data in new and engaging ways, Three.js is a great tool to consider.</p>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- 4. velocity.js -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<p>With Velocity.js, We can use the same API as jQuery’s $.animate() as an animation engine. It is 
compatible with both jQuery and without it. It is extremely fast and features a wide range of 
features, including color animation, transforms, loops, easings, SVG support, and scrolling. It 
combines jQuery and CSS transitions and has the best of both worlds.</p>

<p>In addition, Velocity also offers good compatibility, particularly with older browser platforms. 
Aside from having great documentation, Velocity.js also has a great community willing to help you 
if you require assistance.</p>

<p>Below are some examples of animation made with velocity.js</p>

```
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
```

```
<div class="loader">
      <div class="box"></div>
      <div class="text">Welcome</div>
      <div class="shadow"></div>
    </div>
```

```
<!-- css -->

@import url('https://fonts.googleapis.com/css2?family=Dancing+Script&family=Dosis:wght@300&display=swap');

body {
  background: gray;
}
.loader {
  width: 150px;
  height: 150px;
  display: block;
  margin: 100px auto 0;
  position: relative;
}

.text {
  font-family: 'Dancing Script', cursive;
  text-align: center;
  font-size: 28px;
  color: white;
  z-index: 9;
  position: relative;
  padding: 50px 0 0 0;
}

.shadow {
  position: relative;
  height: 6px;
  border-radius: 50%;
  background-color: #1c1818;
  margin: 100px 0 0 0;
}

.box {
  display: block;
  width: 150px;
  height: 150px;
  background: #153149;
  position: absolute;
  borderRadius: "50px",
  top: 0;
}
```

```
 // velocity.js

$(document).ready(function() {

  function loader() {
    var color = "#9fcbe8";

    $('.box')
    .velocity({
        rotateY: "360deg",
        borderRadius: "50%",
        scale: 0.5,
        backgroundColor: color
    },
    {duration: 1600,
      loop: true,
      easing: [0.750, 0.000, 0.500, 1.000]
    });

    $('.text')
    .velocity({
      rotateY: "360deg",
      scale: 0.5,
      translateY: "38px"
    },
    {duration: 1600,
      loop: true,
      easing: [0.750, 0.000, 0.500, 1.000]
    });

    $('.shadow')
    .velocity({
      scale: 0.5,
      translateY: "0px"
    },
    {duration: 1600,
      loop: true,
      easing: "liner"
    });
  }

  loader();

});
```

<p>I would say that Velocity.js is one of the most powerful and efficient tools for creating smooth 
and performant animations on the web, and I highly recommend it. Even though it may not be the best 
choice for every situation, it is definitely worth considering if you are looking for an animation 
library that is fast and cross-browser compatible.</p>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- 4. GreenSock.js -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<p>GSAP is a popular JavaScript library that makes it easy to create high-performance animations on 
the web. Its optimized code and smart techniques ensure smooth, lag-free animations on all major 
browsers, including mobile devices. GSAP also offers a variety of pre-built tools and functions that 
make it simple for developers to create complex animations quickly and easily, even if they are new 
to web animation. Overall, GSAP is a versatile and powerful platform for creating web animations.</p>

<p>One of the key benefits of GSAP is its ability to create high-performance animations. Its optimized 
codebase and smart techniques ensure that your animations run smoothly and don’t cause lag or jitter. 
This is especially important on mobile devices, where resources are often limited. Another advantage 
of GSAP is its simplicity. The platform includes a wide range of pre-built tools and functions that make 
it easy for developers to create complex animations quickly and easily. Even if you’re new to web 
animation, you can get up and running with GSAP in no time.</p>

```
<!-- html -->

<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.5.1/gsap.min.js"></script>

<button id="replay-button">Replay</button>
<div id="box" class="box">Animate me!</div>
```

```
 // gsap.js

var animation = TweenMax.to("#box", 1, {
  width: 200,
  height: 200,
  backgroundColor: "blue",
  ease: Power1.easeInOut
});

document.getElementById('replay-button').addEventListener('click', function() {
  animation.restart();
});
```

<p>This is a basic example, but GSAP offers many more options and features for creating complex and 
sophisticated animations. You can learn more about using GSAP by reading the documentation and tutorials 
on the GSAP website.</p>

<p>Overall, GSAP is a powerful tool that allows developers to create smooth and performant animations on 
the web. Whether you’re an experienced web developer or just starting out, GSAP is a great platform to 
consider for your next animation project. Below are some examples of animation made with GSAP.js</p>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<!-- 5. Mo.js -->
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->

<p>JavaScript motion graphics library Mo.js is fast, retina-ready, modular, and open source. The syntax 
of this library and how code animations are structured are different from those of other libraries. 
As a result of the declarative API, the animation is entirely customizable, which makes it easy to 
create new animations.</p>

<p>There are built-in components in this library to help you start animating from scratches, such as 
HTML and shape and swirls, bursts, and staggers, but there are also tools to help you craft your 
animation naturally. Mo.js allows you to create delightful animations with accuracy, enhance the 
user experience, and enrich your content visually on your site.</p>

<p>Below are some examples of animation made with Mo.js</p>

```
<script src="https://cdnjs.cloudflare.com/ajax/libs/mo-js/0.288.1/mo.min.js"></script>
```

```
 // mo.js

var shape2 = new mojs.Shape({
  shape : 'polygon',
  points:       4,
  radius : 60,
  left:'50 %',

  isShowStart : true,
  fill: {'#bf3030':'#a11260'},
  delay : 400,
  easing: 'sin.out',
  scale: {0 : 1} ,
  duration : 350,
   backwardEasing: 'sin.in',
  yoyo:  true,


}).play();

var shape4 = new mojs.Shape({
  shape : 'polygon',
  points:       4,
  radius: 150,
  fill: 'transparent',
  strokeWidth:{11:2},
  stroke:'#34495e',
  easing : 'sin.out',
  strokeDasharray: '100%',
  strokeDashoffset: {'100%': '300%'},
  delay : 800,
  duration:1500,
  repeat : 2000000

}).play();

var shape4 = new mojs.Shape({
  shape : 'polygon',
  points:       4,
  radius: 130,
  fill: 'transparent',
  strokeWidth:{11:2},
  stroke:'#34495e',
  easing : 'sin.out',
  strokeDasharray: '100%',
  strokeDashoffset: {'100%': '300%'},
  delay : 1050,
  left:'50 %',
  duration:1500,
  repeat : 20000000

}).play();

var shape4 = new mojs.Shape({
  shape : 'polygon',
  points:       4,
  radius: 110,
  fill: 'transparent',
  strokeWidth:{11:2},
  stroke:'#34495e',
  easing : 'sin.out',
  strokeDasharray: '100%',
  strokeDashoffset: {'100%': '300%'},
  delay : 950,
  duration:1500,
  repeat : 2000000

}).play();

var shape4 = new mojs.Shape({
  shape : 'polygon',
  points:       4,
  radius: 90,
  fill: 'transparent',
  strokeWidth:{11:2},
  stroke:'#34495e',
  easing : 'sin.out',
  strokeDasharray: '100%',
  strokeDashoffset: {'-100%': '-300%'},
  delay : 850,
  duration:1500,
  repeat : 2000000

}).play();

var shape4 = new mojs.Shape({
  shape : 'polygon',
  points:       4,
  radius: 70,
  fill: 'transparent',
  strokeWidth:{11:2},
  stroke:'#34495e',
  easing : 'sin.out',
  strokeDasharray: '100%',
  strokeDashoffset: {'-100%': '-300%'},
  delay : 750,
  duration:1500,
  repeat : 200000

}).play();

new MojsPlayer({ add: timeline, isPlaying: true, isRepeat: true });
```

<p>Overall, Mo.js is a powerful and versatile tool for creating complex and engaging animations on 
the web. Whether you’re a web developer looking to create interactive experiences or a designer 
looking to add some visual flair to your website, Mo.js is a great library to consider.</p>

<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
Summary
<!--~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~-->
<p>In this article, we looked at different JavaScript animation libraries which you can use while 
building a website or web app. There are many libraries out there but we focused on these 5 for now. 
Before we conclude, let’s look at a summary of these libraries.</p>

<p>Anime js: this is a JavaScript animation library that allows making animations with a simple yet 
powerful API. It is one of the best animation libraries of JavaScript.</p>

<p>Three js: this is a powerful 3d animation library in JavaScript that makes running 3d easy in 
JavaScript, it has several features and functions to help make awesome 3d animations.</p>

<p>Velocity js: if you are looking to do animations but not with jquery, you have Velocity js to 
help you out here, and it is also fast.</p>

<p>GreenSock js: this is a smooth animation library for building responsive, accessible-friendly 
animations.</p>

<p>Mo js: This is another excellent motion animation library in JavaScript, it has several good 
features, and it is entirely customizable.</p>

<p>In short, these five libraries are one of the most useful libraries you can find on the internet 
for making animations.</p>
