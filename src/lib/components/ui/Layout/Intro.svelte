<script lang="ts">
	import { SquareArrowOutUpRight, Ellipsis } from 'lucide-svelte';
	import * as Avatar from '$lib/components/ui/avatar';

	let value = 'Follow';
	let isActive = false;
	const clickHandler = () => {
		isActive = true;
		setTimeout(() => {
			value = value === 'Followed' ? 'Follow' : 'Followed';
			isActive = false;
		}, 600);
	};
</script>

<main class="mx-auto my-4 max-w-screen-md py-2">
	<div class="my-4 flex items-center gap-4">
		<section class="mr-4 flex flex-col items-center gap-2">
			<div>
				<Avatar.Root class="h-36 w-36 rounded-full border-4 border-gray-200">
					<Avatar.Image src="/picture.jpeg" alt="Krishna Kiran" />
					<Avatar.Fallback>Krishan Kiran</Avatar.Fallback>
				</Avatar.Root>
			</div>
			<div class="flex flex-col items-center text-lg font-bold">
				<span>Krishan</span>
				<span>Kiran</span>
			</div>
		</section>

		<section>
			<section class="mb-5 flex">
				<div class="p-4">
					Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of
					Engineering. I write hot-takes on building a business, shipping delightful products and
					accelerating product and career growth.
				</div>
				<div>
					<section class="flex w-40 flex-col items-end gap-1">
						<img src="/logo.png" alt="" class="h-10 w-10" />
						<span class="font-bold">Duggup</span>
						<span class="text-sm font-light">Co-Founder and CEO</span>
					</section>
				</div>
			</section>
			<section class="flex justify-between pl-4">
				<div>
					<div
						on:click={clickHandler}
						class={`btn flex cursor-pointer items-center justify-between gap-2 rounded-md px-4 py-2 select-none ${isActive ? 'color bg-blue-600 text-white shadow-none' : ''}`}
					>
						{value}
					</div>
				</div>
				<div class="flex items-center">
					<span class="mr-1 cursor-pointer">My Website</span>
					<SquareArrowOutUpRight class="h-5 w-5 cursor-pointer" />
					<Ellipsis class="ml-4 h-7 w-7 cursor-pointer" color="#bbb" />
				</div>
			</section>
		</section>
	</div>
</main>

<style>
	.btn {
		border: 1px solid #000;
		box-shadow: 0px 4px #000;
		transition: all 200ms linear;
	}
	.btn:hover,
	.btn:active {
		box-shadow: 0px 2px #000;
	}
</style>
