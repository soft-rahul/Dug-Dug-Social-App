<script lang="ts">
	import {CARDS_TEXT} from '../lib/constants/data';
	import Job from '$lib/components/ui/Layer/Job.svelte';
	import Card from '$lib/components/ui/Layer/Card.svelte';
	import Designation from '$lib/components/ui/Layer/Designation.svelte';
	import Point from '$lib/components/ui/Layer/Point.svelte';
</script>

<main class="mx-auto my-2 px-10 py-2 box">
	<section class="grid-container">
		<div class="self-center justify-self-end flex gap-3 items-center mr-7">
			<Point/>
		</div>
		<div></div>
		<div class="flex gap-10">
			<Card image="/jobs.jpeg" description={CARDS_TEXT[0]} />
			<Card image="/sam.jpeg" description={CARDS_TEXT[1]} />
		</div>
		<Job name="Duggup" imageUrl="/logo.png" joinedDate="Nov 2023" />
		<div></div>
		<Designation text="Co-Founder and CEO" jobType="Full-time * Remote " />
		<div class="self-center justify-self-end flex gap-3 items-center mr-7">
			<Point/>
		</div>
		<div></div>
		<div class="flex gap-10">
			<Card image="/setup.jpeg" description={CARDS_TEXT[2]} />
			<Card image="/tokyo.png" description={CARDS_TEXT[3]} />
		</div>
		<Job name="BetterUp" imageUrl="/logoTwo.jpeg" joinedDate="Sep 2022" />
		<div ></div>
		<Designation text="VP Engineering" jobType="Full-time" />
	</section>
</main>

<style>
	.grid-container {
		display: grid;
		grid-template-columns: 1fr 40px 3fr;
		grid-template-rows: auto;
		grid-column-gap: 1rem;
		grid-row-gap: 2rem;
		position: relative;
	}
	.grid-container::after {
		content: '';
		display: block;
		position:absolute;
		top: 0;
		bottom: 0;
		left: 206px;
		border-left: 2px dotted #3f3e4641;
	}
	.box {
		max-width: 1130px;
	}
</style>
