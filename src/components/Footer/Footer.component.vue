<template>
  <footer class="footer">
			<p>Questions? Call 1-866-579-7172</p>
			<div class="footer-cols">
				<ul>
					<li v-for="item in items" :key="item.id"><a href="#">{{item.title}}</a></li>
				</ul>
				<ul>
					<li v-for="list in lists" :key="list.id"><a href="#">{{list.title}}</a></li>
				</ul>
				<ul>
					<li v-for="link in links" :key="link.id"><a href="#">{{link.title}}</a></li>
				</ul>
				<ul>
					<li v-for="notice in notices" :key="notice.id"><a href="#">{{notice.title}}</a></li>
				</ul>
			</div>

		</footer>
</template>

<script>
export default {
	name: "Footer",
	data() {
	return {
		items: [
			{id: 1, title: 'FAQ'},
			{id: 2, title: 'Investor Relations'},
			{id: 3, title: 'Ways To Watch'},
			{id: 4, title: 'Corporate Information'},
			{id: 5, title: 'Netflix Originals'}
			],

		lists:[
			{id: 1, title: 'Help Center'},
			{id: 2, title: 'Jobs'},
			{id: 3, title: 'Terms Of Use'},
			{id: 4, title: 'Contact Us'}
			],

		links: [
			{id: 1, title: 'Account'},
			{id: 2, title: 'Redeem Gift Cards'},
			{id: 3, title: 'Privacy'},
			{id: 4, title: 'Speed Test'}
			],

		notices: [
			{id: 1, title: 'Media Center'},
			{id: 2, title: 'Buy Gift Cards'},
			{id: 3, title: 'Cookie Preferences'},
			{id: 4, title: 'Legal Notices'}
			]
		}
	}
}
</script>

<style scoped>
  .footer {
	max-width: 70%;
	margin: 1rem auto;
	overflow: auto;
}

.footer,
.footer a {
	color: #999;
	font-size: 0.9rem;
}

.footer p {
	margin-bottom: 1.5rem;
}

.footer .footer-cols {
	display: grid;
	grid-template-columns: repeat(4, 1fr);
	grid-gap: 2rem;
}

.footer li {
	line-height: 1.9;
}

.footer .lang-select {
	margin-top: 2rem;
	color: #999;
	background-color: #000;
	background-image: none;
	border: 1px solid #333;
	padding: 1rem 1.2rem;
	border-radius: 5px;
}
</style>
