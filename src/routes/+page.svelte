<script lang="ts">
	import {CARDS_TEXT} from '../lib/constants/data';
	import Job from '$lib/components/ui/Layer/Job.svelte';
	import Card from '$lib/components/ui/Layer/Card.svelte';
	import Designation from '$lib/components/ui/Layer/Designation.svelte';
</script>

<main class="mx-auto my-2 max-w-screen-lg px-10 py-2">
	<section class="grid-container">
		<div class="self-center justify-self-end">
			<span class="text-sm font-light"> Dec 2023</span>
		</div>
		<div class="relative mx-4 bg-gray-100"></div>
		<div class="flex gap-10">
			<Card image="/jobs.jpeg" description={CARDS_TEXT[0]} />
			<Card image="/sam.jpeg" description={CARDS_TEXT[1]} />
		</div>
		<Job name="Duggup" imageUrl="/logo.png" joinedDate="Nov 2023" />
		<div class="relative mx-4 bg-gray-100"></div>
		<Designation text="Co-Founder and CEO" jobType="Full-time * Remote " />
		<div class="self-center justify-self-end">
			<span class="text-sm font-light"> Dec 2023</span>
		</div>
		<div class="relative mx-4 bg-gray-100"></div>
		<div class="flex gap-10">
			<Card image="/setup.jpeg" description={CARDS_TEXT[2]} />
			<Card image="/tokyo.png" description={CARDS_TEXT[3]} />
		</div>
		<Job name="BetterUp" imageUrl="/logoTwo.jpeg" joinedDate="Sep 2022" />
		<div class="relative mx-4 bg-gray-100"></div>
		<Designation text="VP Engineering" jobType="Full-time" />
	</section>
</main>

<style>
	.grid-container {
		display: grid;
		grid-template-columns: 1fr 5px 3fr;
		grid-template-rows: auto;
	}
</style>
