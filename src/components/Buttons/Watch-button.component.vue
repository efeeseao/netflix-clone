<template>
  <div>
    <a href="#" class="btn btn-xl">
      Watch Free For 30 Days <i class="fas fa-chevron-right btn-icon"></i>
    </a>
  </div>
</template>

<script>
export default {
  name: 'WatchButton',
}
</script>

<style scoped>
  .btn {
	display: inline-block;
	background: #e50914;
	color: #fff;
	padding: 0.4rem 1.3rem;
	font-size: 1rem;
	text-align: center;
	border: none;
	cursor: pointer;
	margin-right: 0.5rem;
	transition: opacity 0.2s ease-in;
	outline: none;
	box-shadow: 0 1px 0 rgba(0, 0, 0, 0.45);
	border-radius: 2px;
  }

  .btn:hover {
    opacity: 0.9;
  }

  .btn-xl {
    font-size: 2rem;
    padding: 1.5rem 2.1rem;
    text-transform: uppercase;
  }

  .btn-lg {
    font-size: 1rem;
    padding: 0.8rem 1.3rem;
    text-transform: uppercase;
  }

  .btn-icon {
    margin-left: 1rem;
  }
</style>
