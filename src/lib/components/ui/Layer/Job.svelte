<script lang="ts">
	export let name: string;
	export let imageUrl: string;
	export let joinedDate: string;
	import { ChevronUp } from 'lucide-svelte';
</script>

<section class="relative flex items-center gap-5">
	<div class="flex w-full flex-col">
		<div class="flex flex-col items-end">
			<img src={imageUrl} alt="" class="h-10 w-10 rounded-full" />
			<span class="font-bold">{name}</span>
		</div>
		<div class="flex flex-col items-end">
			<span class="text-nowrap text-sm font-light"> San Francisco Bay Area</span>
			<span class="text-sm font-light">Joined</span>
			<span class="text-sm font-light">{joinedDate}</span>
		</div>
	</div>
	<div class="z-50">
		<div class="-mt-3 mr-4 bg-white">
			<div class="h-10 w-10 rounded-full border-8 border-blue-600"></div>
		</div>
	</div>
	<div class="absolute -top-6 right-6 z-50 bg-white">
		<ChevronUp color="#bbb" />
	</div>
</section>
