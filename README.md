# confetti.js

A simple confetti animation overlay for your website :)

Just add ```<script src="//feelingunlucky.today/js/confetti.js"></script>``` to your website!

![confetti demo](https://i.imgur.com/Tjc8NvJ.png)

Import the file, then call any of the following available functions:

	startConfetti();       //call to start confetti animation
	stopConfetti();        //call to stop adding confetti
	toggleConfetti();      //call to start or stop the confetti animation depending on whether it's already running
	pauseConfetti();       //call to freeze confetti animation
	resumeConfetti();      //call to unfreeze confetti animation
	toggleConfettiPause(); //call to toggle whether the confetti animation is paused
	removeConfetti();      //call to stop the confetti animation and remove all confetti immediately
	isConfettiPaused();    //call and returns true or false depending on whether the confetti animation is paused
	isConfettiRunning();   //call and returns true or false depending on whether the animation is running

You can configure these parameters:

	maxParticleCount = 150;     //set max confetti count
	particleSpeed = 2;          //set the particle animation speed
	confettiFrameInterval = 20; //the confetti animation frame interval

For a live demo, [click here](https://feelingunlucky.today) and search something, anything :)

The demo uses this function:

	function throwConfetti() {
		maxParticleCount = Math.random() * 100 + 50;
		startConfetti();
		setInterval(function() {
			stopConfetti();
		}, 1200);
	}

Enjoy!
