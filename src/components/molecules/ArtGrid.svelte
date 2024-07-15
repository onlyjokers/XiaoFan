<script>
	import Artwork from '../atoms/Artwork.svelte';
</script>

<h3 class="gap"></h3>
<h3 class="title">隐秩序—2024届跨媒体艺术学院</h3>

<div class="grid-container">
	<div class="grid">
		<Artwork art="1-1" tall />
		<Artwork art="1-2" />
		<Artwork art="1-3" tall />
		<Artwork art="1-4" />
		<Artwork art="1-5" tall/>
		<Artwork art="1-6" tall />
		<Artwork
			art="1-7"
			tall
			shrink
			commission
			subtitle=""
		/>
	</div>
</div>

<h3 class="title">事出有因—家庭编年史课程展</h3>
<div class="grid-container">
	<div class="grid">
		<Artwork art="2-1" tall />
		<Artwork art="2-2" />
		<Artwork art="2-3" tall />
		<Artwork art="2-4" />
		<Artwork art="2-5" tall/>
		<Artwork art="2-6" tall />
		<Artwork
			art="2-7"
			tall
			shrink
			commission
			subtitle=""
		/>
	</div>
</div>

<h3 class="title">室内设计2022</h3>
<div class="grid-container">
	<div class="grid">
		<Artwork art="3-1" tall />
		<Artwork art="3-2" />
		<Artwork art="3-3" tall />
		<Artwork art="3-4" />
		<Artwork art="3-5" tall/>
		<Artwork art="3-6" tall />
		<Artwork
			art="3-7"
			tall
			shrink
			commission
			subtitle=""
		/>
		<Artwork art="3-8" tall />
		<Artwork art="3-9" />
		<Artwork art="3-10" tall />
		<Artwork art="3-11" />
		<Artwork art="3-12" tall />
	</div>
</div>

<h3 class="title">慕山溪引</h3>
<div class="grid-container">
	<div class="grid">
		<Artwork art="4-1" tall />
		<Artwork art="4-2" />
		<Artwork art="4-3" tall />
		<Artwork art="4-4" />
		<Artwork art="4-5" tall/>
		<Artwork art="4-6" tall />
		<Artwork
			art="4-7"
			tall
			shrink
			commission
			subtitle=""
		/>
		<Artwork art="4-8" tall />
		<Artwork art="4-9" />
	</div>
</div>

<style lang="scss">
	@import '../../styles/mixins.scss';

	.grid {
		gap: 0.8rem;
		grid-auto-rows: 230px;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		display: grid;
		grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
		width: min(90%, 72rem);

		@media screen and (max-width: 600px) {
			grid-auto-rows: 125px;
		}

		@media screen and (max-width: 868px) {
			width: min(100%, 75rem);
			gap: 0.2rem;
			grid-template-columns: 1fr 1fr 1fr;
		}

		&:before {
			@include outlineText($content: '&&', $translateX: -40%, $translateY: -160%);

			@media screen and (max-width: 868px) {
				@include outlineText($content: '&&', $translateX: -25%, $translateY: -95%);
			}
		}
	}

	.grid-container {
		display: flex;
		justify-content: center;
		margin-bottom: 4rem;
	}

	.title {
		// gap: 0.8rem;
		// grid-auto-rows: 230px;
		// flex-direction: column;
		// justify-content: center;
		// align-items: center;
		// display: grid;
		// grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
		// width: min(90%, 72rem);

		display: flex;
		justify-content: center;
		// margin-top:10 rem;
		margin-bottom: 4rem;
	}

	.gap {
		// gap: 0.8rem;
		// grid-auto-rows: 230px;
		// flex-direction: column;
		// justify-content: center;
		// align-items: center;
		// display: grid;
		// grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
		// width: min(90%, 72rem);

		display: flex;
		justify-content: center;
		// margin-top:10 rem;
		margin-bottom: 2rem;
	}
</style>
