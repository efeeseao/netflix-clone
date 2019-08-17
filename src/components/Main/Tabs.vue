<template>
  <section class="tab-content">
			<div class="container">
				<!-- Tab Content 1 -->
				<div id="tab-1-content" class="tab-content-item show">
					<div class="tab-1-content-inner">
						<div>
							<p class="text-lg">
								If you decide Netflix isn't for you - no problem. No commitment.
								Cancel online anytime.
							</p>
							<WatchButton />
						</div>
						<img src="https://i.ibb.co/J2xDJV7/tab-content-1.png" alt="" />
					</div>
				</div>
			</div>
		</section>
</template>

<script>
import WatchButton from '../Buttons/Watch-button.component';
export default {
  name: 'Tabs',
  components: {
    WatchButton
  }
}
</script>

<style scoped>
  .tab-content {
	padding: 3rem 0;
	background: #000;
	color: #fff;
}

/* Hide initial content */
#tab-1-content {
	display: none;
	opacity: 0;
}

.show {
	display: block !important;
	opacity: 1 !important;
	transition: all 1000 ease-in;
}

#tab-1-content .tab-1-content-inner {
	display: grid;
	grid-template-columns: repeat(2, 1fr);
	grid-gap: 2rem;
	align-items: center;
	justify-content: center;
}
</style>
