<script>
    import { fade } from "svelte/transition";

    let menuExpanded = false
    const toggleMenu = () => menuExpanded = !menuExpanded
</script>

<div class="flex justify-between px-4 py-2">
    <div class="flex items-center text-gray-600">
        <button class="hover:text-gray-300 transition duration-100">
            <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M12.707 5.293a1 1 0 010 1.414L9.414 10l3.293 3.293a1 1 0 01-1.414 1.414l-4-4a1 1 0 010-1.414l4-4a1 1 0 011.414 0z" clip-rule="evenodd"/></svg>
        </button>
        <button class="hover:text-gray-300 transition duration-100">
            <svg class="w-8 h-8 ml-2" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z" clip-rule="evenodd"/></svg>
        </button>
        <div class="ml-4 relative flex items-center">
            <svg class="absolute ml-2 w-4 h-4 text-gray-800" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M8 4a4 4 0 100 8 4 4 0 000-8zM2 8a6 6 0 1110.89 3.476l4.817 4.817a1 1 0 01-1.414 1.414l-4.816-4.816A6 6 0 012 8z" clip-rule="evenodd"/></svg>
            <input class="pl-8 py-1 text-xs rounded-full placeholder-gray-800 focus:outline-none" placeholder="Search" />
        </div>
    </div>

    <div class="flex items-center text-sm text-gray-200">
        <a href="/" class="flex group items-center">
            <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M18 10a8 8 0 11-16 0 8 8 0 0116 0zm-6-3a2 2 0 11-4 0 2 2 0 014 0zm-2 4a5 5 0 00-4.546 2.916A5.986 5.986 0 0010 16a5.986 5.986 0 004.546-2.084A5 5 0 0010 11z" clip-rule="evenodd"/></svg>
            <span class="ml-1 leading-none group-hover:underline">xgrodx</span>
        </a>
        <div class="relative ml-4">
            <button class="focus:outline-none transform hover:scale-125 transition duration-100" on:click={toggleMenu}>
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 20 20"><path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd"/></svg>
            </button>
            {#if menuExpanded}
                <div transition:fade={{duration:30}} class="absolute w-48 py-2 right-0 z-10 rounded-lg shadow-xl text-gray-400 text-sm bg-gray-700">
                    <a class="block px-4 py-2 hover:text-gray-200 hover:bg-gray-600 transition duration-100" href="/">Hide Activity</a>
                    <a class="block px-4 py-2 hover:text-gray-200 hover:bg-gray-600 transition duration-100" href="/">Account</a>
                    <a class="block px-4 py-2 hover:text-gray-200 hover:bg-gray-600 transition duration-100" href="/">Settings</a>
                    <a class="block px-4 py-2 hover:text-gray-200 hover:bg-gray-600 transition duration-100" href="/">Log Out</a>
                </div>
            {/if}
        </div>
    </div>
</div>