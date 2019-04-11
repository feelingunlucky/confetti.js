# confetti.js

A simple confetti animation overlay for your website :)

Just add ```<script src="confetti.js"></script>``` to your website!

![confetti demo](https://i.imgur.com/Tjc8NvJ.png)

Import the file, then call any of the following available functions:

    startConfetti();     //starts the confetti animation
    stopConfetti();      //stops adding confetti
    toggleConfetti();    //starts or stops the confetti animation depending on whether it's already running
    removeConfetti();    //stops the confetti animation and removes all confetti immediately
    isConfettiRunning(); //call and returns true or false depending on whether the animation is running

You can configure these parameters:

    maxParticleCount = 150; //set max confetti count
    particleSpeed = 2; //set the particle animation speed

For a live demo, [click here](https://feelingunlucky.today) and search something, anything :)

The demo uses this function:

    function throwConfetti() {
        maxParticleCount = Math.random() * 250 + 5;
        startConfetti();
        setInterval(function() {
            stopConfetti();
        }, 1200);
    }

Enjoy!
