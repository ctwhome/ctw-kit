<script>
	import { Hello } from '$lib';
</script>

<div class="bg-base-100 min-h-screen p-8">
	<div class="mx-auto max-w-2xl">
		<h1 class="mb-8 text-3xl font-bold">CTW Kit Component Demo</h1>

		<div class="card bg-base-200 shadow-xl">
			<div class="card-body">
				<h2 class="card-title mb-4">Hello Component</h2>
				<div class="space-y-4">
					<Hello name="World" />
					<Hello name="SvelteKit" />
					<Hello name="Developer" />
				</div>
			</div>
		</div>
	</div>
</div>
