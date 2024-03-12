<script lang="ts">
	import {
		HomeIcon,
		BookOpen,
		AlignVerticalSpaceBetween,
		SquarePlus,
		ChevronDown
	} from 'lucide-svelte';
	import * as Avatar from '$lib/components/ui/avatar';
</script>

<header>
	<div
		class="mx-auto flex items-center border-b-2 border-dotted border-gray-300 px-8 py-4"
	>
		<section class="mr-auto">
			<div class="flex cursor-pointer items-center gap-2">
				<img src="/logo.png" alt="" class="h-6 w-6" />
				<h1 class="text-lg font-bold">Duggup</h1>
			</div>
		</section>
		<section class="flex items-center">
			<div class="flex items-center gap-6 font-light">
				<div class="flex cursor-pointer items-center gap-2">
					<HomeIcon class="h-4 w-4" />
					<div>Home</div>
				</div>
				<div class="flex cursor-pointer items-center gap-2">
					<AlignVerticalSpaceBetween class="h-4 w-4" />
					<div>Explore</div>
				</div>
				<div class="flex cursor-pointer items-center gap-2">
					<BookOpen class="h-4 w-4" />
					<div>Learn</div>
				</div>
			</div>

			<div class="mx-14">
				<div
					class="border-1 btn flex cursor-pointer items-center justify-between gap-2 rounded-md px-4 py-2"
				>
					<SquarePlus class="h-5 w-5" />
					<span> Post </span>
				</div>
			</div>

			<div class="flex items-center gap-2">
				<div class="rounded-full border-2 border-gray-200">
					<Avatar.Root>
						<Avatar.Image src="/picture.jpeg" alt="Krishna Kiran" />
						<Avatar.Fallback>Krishan Kiran</Avatar.Fallback>
					</Avatar.Root>
				</div>
				<div>
					<span class="font-bold">Krishna Krina</span>
				</div>
				<div class="cursor-pointer">
					<ChevronDown class="h-5 w-5" />
				</div>
			</div>
		</section>
	</div>
</header>

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
