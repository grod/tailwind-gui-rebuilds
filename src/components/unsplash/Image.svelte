<script>
    export let image
</script>
<div class="group relative">
    <div class="absolute flex flex-col justify-between inset-0 opacity-0 group-hover:opacity-100 bg-black bg-opacity-25 transition duration-100">
        <div class="flex justify-end px-5 pt-5 space-x-3">
            <button class="px-3 py-2 rounded text-gray-700 hover:text-gray-900 bg-gray-300">
                <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clip-rule="evenodd"></path></svg>
            </button>
            <button class="px-3 py-2 rounded text-gray-700 hover:text-gray-900 bg-gray-300">
                <svg class="w-5 h-5" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M12 4v16m8-8H4"/></svg>
            </button>
        </div>
        <div class="flex justify-between px-5 pb-4">
            <a href="/" class="flex items-center text-gray-300 hover:text-white">
                <img class="w-8 h-8 rounded-full object-cover" src="{image.avatar}" alt="">
                <div class="ml-2 font-normal">{image.author}</div>
            </a>
            <div>
                <button class="px-3 py-2 rounded text-gray-700 hover:text-gray-900 bg-gray-300">
                    <svg class="w-4 h-4" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M19 14l-7 7m0 0l-7-7m7 7V3"/></svg>
                </button>
            </div>
        </div>
    </div>
    <img class="w-full" alt="" src={image.url} />
</div>