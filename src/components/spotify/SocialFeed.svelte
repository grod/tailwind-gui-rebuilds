<script>
    export let socialFeed
</script>

<h2 class="pb-2 border-b border-gray-800 text-lg font-semibold text-gray-200">Friend Activity</h2>

<div class="mt-4 space-y-10">
    {#each socialFeed as item}
        <div class="flex items-center">
            <img class="w-10 h-10 rounded-full object-cover" src={item.avatar} alt="Avatar" />
            <div class="flex-shrink ml-4 text-gray-600 text-xs overflow-x-hidden">
                <a href="/" class="block text-sm font-medium text-gray-200 truncate hover:underline">{item.user}</a>
                <a href="/" class="block mt-1 hover:underline">{item.song}</a>
                <a href="/" class="block hover:underline">{item.artist}</a>
                <div class="mt-1 flex items-center">
                    <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 9a3 3 0 100-6 3 3 0 000 6zm-7 9a7 7 0 1114 0H3z" clip-rule="evenodd"/></svg>
                    <a href="/" class="block ml-1 leading-none hover:underline truncate">{item.album}</a>
                </div>
            </div>
        </div>
    {/each}
</div>

<div class="mt-12 text-center">
    <button class="px-8 py-1 text-xs uppercase tracking-widest border-gray-500 text-gray-300 border-2 rounded-full transform hover:scale-110 hover:text-gray-200 hover:border-gray-300 transition duration-100">Find Friends</button>
</div>
