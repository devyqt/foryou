<!DOCTYPE html>
<html>
<head>
	<title> for my Beautiful Girl</title>
	<style>
		img {
			max-width: 50%;
			height: auto;
			display: block;
			margin: auto;
			margin-top: 50px;
			margin-bottom: 50px;
		}
	</style>
</head>
<body>
	<h1>Hi Mahal!</h1>
	<button onclick="surprise()">Click mo mahal!</button>
	<div id="message"></div>
	<script>
		function surprise() {
			var messages = [
				"You are the sunshine of my life!",
				"I can't imagine my life without you!",
				"You make every day brighter!",
				"You are the most beautiful woman in the world!",
				"I love you more than words can express!"
			];
			var message = messages[Math.floor(Math.random() * messages.length)];

			var img = document.createElement("img");
			img.src = "https://scontent.fmnl30-1.fna.fbcdn.net/v/t1.15752-9/339483719_1028358251901909_2666426708349648565_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=ae9488&_nc_eui2=AeE3RKZ6niX3albimgNIEaTd64DzvCppcezrgPO8Kmlx7GP3vY_FrILoPG991HDu7sltJiIkgxfN-2WaLedxwdAo&_nc_ohc=jaZfz8jxe_UAX98C7O-&_nc_oc=AQlk-253Bw9Da_8ijsedvtG_afDvwj2zDG5Cheu0N_9hjtC1x8pO-roVOAK-2zJKEyE&_nc_ht=scontent.fmnl30-1.fna&oh=03_AdR-jt98tfVfHzQKeY71M8bsQ1fMX87aHgsO_4x3XT2ROg&oe=645E14F7";
			img.alt = "mygirl";

			var p = document.createElement("p");
			p.innerHTML = message;

			var container = document.getElementById("message");
			container.innerHTML = "";
			container.appendChild(img);
			container.appendChild(p);
		}
	</script>
</body>
</html>
