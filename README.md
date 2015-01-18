# HTML5_Training


============================

<!doctype html>
<html lang="en">
<head>
	<meta charset="UTF-8" />
	<title>Document</title>
	<script src="lib/three.js"></script>
	<script>
		// scene
		// camera
		// object
		var scene = new THREE.Scene();
		var camera = new THREE.PerspectiveCamera(75,window.innerWidth/window.innerHeight,1,1000)
		camera.position.z = 400;
		scene.add(camera);
		
		var renderer = window.WebGLRenderingContext ? new THREE.WebGLRenderer() : new THREE.CanvasRenderer();
		renderer.setSize(window.innerWidth,window.innerHeight);
		window.onload = function(){
			document.appendChild(renderer.domElement);
			//====================================
			
			//====================================
		}
		renderer.render(scene,camera);
		
	</script>
</head>
<body>

</body>
</html>