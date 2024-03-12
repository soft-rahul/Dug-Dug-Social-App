<script lang="ts">
	export let name:string;
	export let imageUrl:string;
	export let joinedDate:string;
</script>

<div class="flex w-28 flex-col items-end">
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
