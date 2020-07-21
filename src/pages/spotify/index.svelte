<script>
    import Album from "../../components/spotify/Album.svelte"

    const albums = [
        { artist: 'Beastie Boys', name: 'Check Your Head', art: 'beastie_boys-check_your_head.webp'},
        { artist: 'Weezer', name: 'Van Weezer', art: 'weezer-van_weezer.png'},
        { artist: 'Slayer', name: 'South Of Heaven', art: 'slayer-south_of_heaven.webp'},
        { artist: 'Weezer', name: 'Teal Album', art: 'weezer-teal_album.webp'},
    ]
</script>

<h1 class="mt-10 text-5xl font-semibold text-white">Home</h1>

<section class="mt-8">
    <h2 class="pb-px border-b border-gray-700 text-xl font-medium text-white">Recently Played</h2>
    <div class="mt-5 grid grid-cols-4 gap-4">
        {#each albums as album}
            <Album {album} />
        {/each}
    </div>
</section>
<section class="mt-20">
    <h2 class="pb-px border-b border-gray-700 text-xl font-medium text-white">For those who likes The Beach Boys</h2>
    <div class="mt-5 grid grid-cols-4 gap-4">
        {#each albums as album}
            <Album {album} />
        {/each}
    </div>
</section>
<section class="mt-20">
    <h2 class="pb-px border-b border-gray-700 text-xl font-medium text-white">For those who likes Weezer</h2>
    <div class="mt-5 grid grid-cols-4 gap-4">
        {#each albums as album}
            <Album {album} />
        {/each}
    </div>
</section>
