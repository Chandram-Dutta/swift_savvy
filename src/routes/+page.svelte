<script lang="ts">
	import { goto } from "$app/navigation";
	import { Button } from "bits-ui";

    function openUrl(url: string){
        window.open(url, "_blank");
    }
</script>
<div class="flex flex-col items-center justify-center h-screen">
	<h1 class="text-6xl md:text-9xl font-bold">Swift Savvy</h1>
    <span>By <a class="underline" href="https://onlychan.xyz/">Chandram Dutta</a></span>
    <div class="flex flex-col sm:flex-row m-4 gap-2">
        <Button.Root class="duration-300 transition active:scale-95 hover:bg-white hover:text-orange-500 bg-black text-white rounded-md p-4">
            Udemy
        </Button.Root>
        <Button.Root class="duration-300 transition active:scale-95 hover:bg-white hover:text-orange-500 bg-black text-white rounded-md p-4">
            Youtube
        </Button.Root>
        <Button.Root on:click={()=> goto("/checklist")} class="duration-300 transition active:scale-95 hover:bg-white hover:text-orange-500 bg-black text-white rounded-md p-4">
            Checklist
        </Button.Root>
        <Button.Root on:click={() => openUrl("https://github.com/Chandram-Dutta/GDSC-Swift-Course")} class="duration-300 transition active:scale-95 hover:bg-white hover:text-orange-500 bg-black text-white rounded-md p-4">
            Course Materials
        </Button.Root>
    </div>
    
</div>
