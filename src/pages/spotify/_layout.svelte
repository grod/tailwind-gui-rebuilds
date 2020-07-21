<script>
    import Sidebar from "../../components/spotify/Sidebar.svelte";
    import SocialFeed from "../../components/spotify/SocialFeed.svelte";
    import Player from "../../components/spotify/Player.svelte";
    import TopBar from "../../components/spotify/TopBar.svelte";

    const socialFeed = [
        { user: 'elstudion', song: 'Like Hell Broke Away', artist: 'Lonnie Holley', album: 'Dusha', avatar: 'https://images.unsplash.com/photo-1570045006801-08ec03621a42?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=200&q=80'},
        { user: 'Jackson Holiday Wheeler', song: 'Dusha', artist: 'Tebra', album: 'Dusha', avatar: 'https://images.unsplash.com/photo-1584999734482-0361aecad844?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=300&q=80'},
        { user: 'Miguel Santa Eufèrmia', song: 'Code Of The Streets', artist: 'Gang Starr', album: 'No Half Steppin\'', avatar: 'https://images.unsplash.com/photo-1541647376583-8934aaf3448a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=300&q=80'},
        { user: 'Adrian Berggren', song: 'Det lilla livet', artist: 'Familjen', album: 'Det snurrar i min skalle', avatar: 'https://images.unsplash.com/photo-1579591919791-0e3737ae3808?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=300&q=80'},
    ]

</script>

<div class="flex h-screen flex-col text-gray-500">
    <div class="flex flex-1 overflow-y-hidden">
        
        <div class="flex bg-gray-900">
            <Sidebar />
        </div>

        <div class="flex flex-col flex-1 bg-gray-800 overflow-y-hidden">
            <div class="bg-gray-800">
                <TopBar />
            </div>
            <div class="px-8 py-8 flex-1 overflow-y-auto">
                <slot />
            </div>
        </div>

        <div class="w-56 pt-2 pb-10 px-4 bg-gray-900 overflow-y-auto">
            <SocialFeed {socialFeed} />
        </div>

    </div>

    <div class="bg-gray-700">
        <Player />
    </div>

</div>