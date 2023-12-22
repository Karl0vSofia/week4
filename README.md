<html>
  <head>
    <script src="aframe/aframe.min.js"></script> 
    <script src="https://cdn.jsdelivr.net/gh/c-frame/aframe-extras@7.0.0/dist/aframe-extras.min.js"></script>
  </head>
  <body>
	<a-scene stats>
<meta charset="utf-8">
  <title>Привязка фигур к маркерам</title>
  <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
</head>
<body>
  <a-scene>
    
    <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
    
  
    <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
    
   
    <a-cylinder position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
      </a-scene>

<a-marker preset="hiro">

  <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
</a-marker>



<a-marker preset="kanji">

  <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
</a-marker>


<a-marker preset="custom">

  <a-cylinder position="1 0.75 -3" radius="0.5" height="1.5" color="#FFC65D"></a-cylinder>
</a-marker>
<a-marker id="marker1" preset="hiro" emitevents="true">
  <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"
         animation__markerfound="property: scale; to: 2 2 2; dur: 500"
         animation__markerlost="property: scale; to: 1 1 1; dur: 500">
  </a-box>
</a-marker>
<a-marker id="marker2" preset="kanji" emitevents="true">
  <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E""
         animation__markerfound="property: scale; to: 2 2 2; dur: 500"
         animation__markerlost="property: scale; to: 1 1 1; dur: 500">
  </a-sphere>
</a-marker>
</a-marker>
<a-marker id="marker3" preset="custom" emitevents="true">
	<a-marker preset="custom" type="pattern" url="../SonyaIT/Apple_Store_logo.svg">
  <a-cylinder position="0 1.25 -5" radius="1.25" color="#EF2D5E""Z
         animation__markerfound="property: scale; to: 2 2 2; dur: 500"
         animation__markerlost="property: scale; to: 1 1 1; dur: 500">
  </a-cylinder->
</a-marker>

	</a-scene>
  </body>
</html>
