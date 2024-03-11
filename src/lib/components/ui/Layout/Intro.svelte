<script lang="ts">
    import {SquareArrowOutUpRight, Ellipsis} from 'lucide-svelte';
	import * as Avatar from '$lib/components/ui/avatar';
</script>

<main class="mx-auto my-6 max-w-screen-lg px-10 py-2">
	<div class="my-4 flex items-center gap-4">
		<section class="mr-4 flex flex-col items-center gap-2">
			<div>
				<Avatar.Root class="h-36 w-36 rounded-full border-2 border-gray-100">
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
			<section class="flex">
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
						class="flex cursor-pointer items-center justify-between gap-2 rounded-md border-2 border-gray-600 px-4 py-2 hover:border-gray-200"
					>
						Follow
					</div>
				</div>
				<div class="flex items-center">
                    <span>My Website</span>
                    <SquareArrowOutUpRight class="w-5 h-5"/>
                    <Ellipsis class="h-7 w-7 ml-4" color="#bbb"/>
                </div>
			</section>
		</section>

		<section></section>
	</div>
</main>
