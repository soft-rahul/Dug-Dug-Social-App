<script lang="ts">
    export let  text:string;
    export let jobType:string;
</script>

<div class="bg-white p-4 border shadow-md rounded-md self-center ">
    <span class="font-bold text-lg">{text}</span>
    <span class="font-light text-sm flex items-center ">{jobType}</span>
</div>