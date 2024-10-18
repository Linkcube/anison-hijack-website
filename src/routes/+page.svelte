<video autoplay={true} muted={true} loop={true}>
	<source src="/background.webm" type="video/webm" />
</video>
<main>
	<div class="intro-text">
		<p>
			Anison Hijack is a collective of DJs specializing in otaku-centric music including anime,
			video games, Japanese dance, hardstyle, and more. We run biweekly shows on Twitch as well as
			occasional larger festivals and events year-round. We frequently collaborate with other DJ
			groups and host guests from around the world on our shows as well. For more information and
			archives of past shows, please visit us at <a href="https://twitter.com/AnisonH">Twitter</a>
			or <a href="https://twitch.tv/anisonhijack">Twitch</a>.
		</p>
	</div>

	<div class="twitch-container">
		<iframe
			src="https://player.twitch.tv/?channel=anisonhijack&amp;parent=localhost"
			scrolling="no"
			allow="fullscreen"
			width="640"
			height="360"
			title="Twitch Page"
		>
		</iframe>
	</div>
</main>

<style>
	main {
		display: flex;
		flex-direction: column;
		justify-content: start;
	}

	.twitch-container {
		margin-left: auto;
		margin-right: auto;
		margin-top: 100px;
	}

	.intro-text {
		margin-left: auto;
		margin-right: auto;
		width: 80%;
	}

	video {
		z-index: -1;
		position: fixed;
		top: 0;
		left: 0;
		min-width: 100%;
		min-height: 100%;
		transform: translateX(calc((100vw - 100%) / 2));
	}
</style>
