<h1>This is the main component</h1>

<!--
<div>
	<p>
		This is the yielding component outside of an each loop:
	</p>
	<Yielder>
		Hello {{people[0]}}
	</Yielder>
</div>
-->

<div>
	{{#each people as person}}
	<p>
		Gonna say hi to {{person}} inside this yielding component
	</p>
	<Yielder>
		Hello {{person}}
	</Yielder>
	{{/each}}
</div>

<script>
export default {
	data: () => ({
		people: [
			'world',
			'bob'
		]
	}),
	components: {
		Yielder
	}
}
</script>
