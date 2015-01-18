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
			document.body.appendChild(renderer.domElement);
		}
		//====================================
		// your code comes here
		
		/*
		var shape = new THREE.SphereGeometry(100, 24, 24);
		var cover = new THREE.MeshNormalMaterial();
		var ball = new THREE.Mesh(shape, cover);
		scene.add(ball);
		 */
		
		// donut
		// cylinder
		
		var shape = new THREE.BoxGeometry(100,100,100);
		var cover = new THREE.MeshNormalMaterial();
		var box = new THREE.Mesh(shape, cover);
		box.position.set(0,0,-50);
		box.rotation.set(15,0,0);
		scene.add(box);
		
		
		//====================================
		renderer.render(scene,camera);
		
	</script>
</head>
<body>

</body>
</html>