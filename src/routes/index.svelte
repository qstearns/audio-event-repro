<script>
    let myDuration = 0
</script>


<svelte:head>
	<title>The duration seems off.</title>
</svelte:head>

<p>
    The duration of this audio is {myDuration}.
</p>

<audio
	controls
	bind:duration={myDuration}
	on:durationchange={() => console.log("the duration changed")}
	src="https://media.transistor.fm/4bfbd3c7.mp3" />
