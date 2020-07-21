<script>
    export let album
</script>

<div class="block">
    <div class="group relative">
        <img class="w-full" src={album.art} alt={album.name} />

        <div class="p-4 absolute flex items-center justify-between inset-0 bg-black bg-opacity-50 text-gray-400 opacity-0 group-hover:opacity-100 transition duration-150">
            <button class="transform hover:scale-110 hover:text-gray-200 transition duration-100">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M3.172 5.172a4 4 0 015.656 0L10 6.343l1.172-1.171a4 4 0 115.656 5.656L10 17.657l-6.828-6.829a4 4 0 010-5.656z" clip-rule="evenodd"/></svg>
            </button>
            <button class="transform hover:scale-110 hover:text-gray-200 transition duration-100">
                <svg class="w-20 h-20" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z" clip-rule="evenodd"/></svg>
            </button>
            <button class="transform hover:scale-110 hover:text-gray-200 transition duration-100">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20"><path d="M6 10a2 2 0 11-4 0 2 2 0 014 0zm6 0a2 2 0 11-4 0 2 2 0 014 0zm4 2a2 2 0 100-4 2 2 0 000 4z"/></svg>
            </button>
        </div>
    </div>
    <a href="/" class="block mt-2 text-white text-sm font-medium hover:underline">{album.name}</a>
    <a href="/" class="block mt-1 text-xs hover:underline">{album.artist}</a>
</div>