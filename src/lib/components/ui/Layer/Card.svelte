<script lang="ts">
	export let description: string;
	export let image: string;
</script>

<section class="flex w-2/4 flex-col rounded-lg border shadow-sm">
	<div class="h-40 w-full">
		<img
			src={image}
			alt="steve jobs"
			class="h-full w-full rounded-tl-lg rounded-tr-lg object-cover"
		/>
	</div>
	<div class="p-4">
		{description}
	</div>
</section>
