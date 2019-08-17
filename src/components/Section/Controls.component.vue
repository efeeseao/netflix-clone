<template>
  <section class="controls">
			<div class="container">
				<div id="tab-1" class="control-item control-border">
					<i class="fas fa-door-open fa-3x"></i>
					<p>Cancel at any time</p>
				</div>
				<div id="control-2" class="control-item">
					<i class="fas fa-tablet-alt fa-3x"></i>
					<p>Watch anywhere</p>
				</div>
				<div id="control-3" class="control-item">
					<i class="fas fa-tags fa-3x"></i>
					<p>Pick your price</p>
				</div>
			</div>
		</section>
</template>

<script>
export default {
  name: 'Controls'

}
</script>

<style scoped>
  .controls {
    background: #141414;
    padding-top: 1rem;
    border-bottom: 3px solid #3d3d3d;
    border-right: none;
  }

  .controls .container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-gap: 1rem;
    align-items: center;
    justify-content: center;
    text-align: center;
  }

  .controls p {
    font-size: 1.2rem;
    padding-top: 0.5rem;
  }

  .controls .container > div {
    padding: 1.5rem 0;
  }

  .controls .container > div:hover {
    color: #fff;
    cursor: pointer;
  }

  .control {
    border-bottom: #e50914 4px solid;
  }

  .container {
	max-width: 70%;
	margin: auto;
	overflow: hidden;
	padding: 0 2rem;
}

</style>
