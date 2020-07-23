<script>
    const files = [
        { name: 'public', type: 'folder', commit: 'Initial commit', timeAgo: '2 days ago' },
        { name: 'src', type: 'folder', commit: 'Hover states', timeAgo: '13 minutes ago' },
        { name: '.gitignore', commit: 'Initial commit', timeAgo: '2 days ago' },
        { name: 'README', commit: 'Created README', timeAgo: '3 minutes ago' },
        { name: 'index.html', commit: 'noindex', timeAgo: '2 days ago' },
        { name: 'package-lock.json', commit: 'Initial commit', timeAgo: '2 days ago' },
        { name: 'package.json', commit: 'removed firebase configs', timeAgo: '2 days ago' },
        { name: 'postcss.config.js', commit: 'Initial commit', timeAgo: '2 days ago' },
        { name: 'routify.config.js', commit: 'Initial commit', timeAgo: '2 days ago' },
        { name: 'svelte.config.js', commit: 'Initial commit', timeAgo: '2 days ago' },
        { name: 'tailwind.config.js', commit: 'Added Netlify', timeAgo: 'yesterday' },
        { name: 'tailwind.default.config.js', commit: 'Initial commit', timeAgo: '2 days ago' },
        { name: 'vite.config.js', commit: 'Initial commit', timeAgo: '2 days ago' },
    ]
</script>

<div class="flex justify-between">
    <div class="flex items-center space-x-4">
        <button class="flex items-center px-4 py-1 rounded-md border font-medium text-sm border-gray-400 bg-gray-100 hover:bg-gray-200">
            <svg class="w-4 h-4 text-gray-700" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M8.684 13.342C8.886 12.938 9 12.482 9 12c0-.482-.114-.938-.316-1.342m0 2.684a3 3 0 110-2.684m0 2.684l6.632 3.316m-6.632-6l6.632-3.316m0 0a3 3 0 105.367-2.684 3 3 0 00-5.367 2.684zm0 9.316a3 3 0 105.368 2.684 3 3 0 00-5.368-2.684z"></path></svg>
            <div class="ml-2">master</div>
            <svg class="ml-2 w-3 h-3" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M19 9l-7 7-7-7"/></svg>
        </button>
        <a href="/" class="group flex items-center text-sm hover:text-blue-600">
            <svg class="w-4 h-4 text-gray-700 group-hover:text-blue-600" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M8.684 13.342C8.886 12.938 9 12.482 9 12c0-.482-.114-.938-.316-1.342m0 2.684a3 3 0 110-2.684m0 2.684l6.632 3.316m-6.632-6l6.632-3.316m0 0a3 3 0 105.367-2.684 3 3 0 00-5.367 2.684zm0 9.316a3 3 0 105.368 2.684 3 3 0 00-5.368-2.684z"></path></svg>
            <span class="ml-1 font-semibold">1</span>
            <span class="ml-1 text-gray-600 group-hover:text-blue-600">branch</span>
        </a>
        <a href="/" class="group flex items-center text-sm hover:text-blue-600">
            <svg class="w-4 h-4 text-gray-700 group-hover:text-blue-600" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M7 7h.01M7 3h5a1.99 1.99 0 011.414.586l7 7a2 2 0 010 2.828l-7 7a2 2 0 01-2.828 0l-7-7A1.994 1.994 0 013 12V7a4 4 0 014-4z"/></svg>
            <span class="ml-1 font-semibold">0</span>
            <span class="ml-1 text-gray-600 group-hover:text-blue-600">tags</span>
        </a>
    </div>

    <div class="flex space-x-2">
        <button class="flex items-center px-4 py-1 rounded-md border font-medium text-sm border-gray-400 bg-gray-100 hover:bg-gray-200">
            <div>Go to file</div>
        </button>
        <button class="flex items-center px-4 py-1 rounded-md border font-medium text-sm border-gray-400 bg-gray-100 hover:bg-gray-200">
            <div>Add file</div>
            <svg class="ml-1 w-3 h-3" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M19 9l-7 7-7-7"/></svg>
        </button>
        <button class="flex items-center px-4 py-1 rounded-md border font-medium text-sm text-green-100 border-green-700 bg-green-600 hover:bg-green-700">
            <svg class="w-4 h-4 text-white" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M4 16v1a3 3 0 003 3h10a3 3 0 003-3v-1m-4-4l-4 4m0 0l-4-4m4 4V4"/></svg>
            <div class="ml-2">Code</div>
            <svg class="ml-1 w-3 h-3" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M19 9l-7 7-7-7"/></svg>
        </button>
    </div>
</div>

<div class="flex justify-between px-3 py-4 mt-4 border rounded-t-md border-blue-200 bg-blue-100">
    <div class="flex items-center">
        <img class="w-6 h-6" src="grod-avatar.png" alt="" />
        <div class="ml-3 text-sm">
            <span class="font-semibold">grod</span> removed firebase configs
        </div>
    </div>
    <div class="flex items-center space-x-2 text-sm text-gray-600">
        <div class="-mb-1 font-mono text-xs">9f2a400</div>
        <div>2 days ago</div>
        <div class="flex items-center">
            <svg class="ml-1 w-5 h-5" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
            <span class="ml-1 font-semibold text-gray-800">6</span>
            <span class="ml-1">commits</span>
        </div>
    </div>
</div>


{#each files as file, i}
<div class="flex justify-between border border-t-0 px-3 py-2 text-sm hover:bg-gray-100 {i === files.length - 1 && 'rounded-b-md'}">
    <div class="flex items-center w-56">

        {#if file.type === 'folder'}
            <svg class="w-5 h-5 text-blue-400" fill="currentColor" viewBox="0 0 20 20"><path d="M2 6a2 2 0 012-2h5l2 2h5a2 2 0 012 2v6a2 2 0 01-2 2H4a2 2 0 01-2-2V6z"/></svg>
        {:else}
            <svg class="w-5 h-5 text-gray-600" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M7 21h10a2 2 0 002-2V9.414a1 1 0 00-.293-.707l-5.414-5.414A1 1 0 0012.586 3H7a2 2 0 00-2 2v14a2 2 0 002 2z"/></svg>
        {/if}
        <div class="ml-3">{file.name}</div>
    </div>
    <div class="flex-1 text-gray-600">{file.commit}</div>
    <div class="text-gray-600">{file.timeAgo}</div>
</div>
{/each}

<div class="flex justify-between mt-4 px-4 py-4 space-x-20 text-sm border rounded-md border-blue-400 bg-blue-200">
    <div>Help people interested in this repository understand your project by adding a README.</div>
    <div>
        <button class="px-3 py-1 font-medium text-xs rounded text-white whitespace-no-wrap bg-green-600 hover:bg-green-700">Add a README</button>
    </div>
</div>