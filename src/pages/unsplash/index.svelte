<script>
import Image from "../../components/unsplash/Image.svelte";

    const imagesLeft = [
        { 
            url: 'https://images.unsplash.com/photo-1595255676545-7c1be5a3b809?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'John Fornander',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595230404149-3ec41df33d5d?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'Philipp Deiß',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595320260530-f3b188507214?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80',
            author: 'Jonathan Leppan',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595148536784-9efae57adced?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'Logan Weaver',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
    ]

    const imagesCenter = [
        { 
            url: 'https://images.unsplash.com/photo-1595312232386-1e5651fd84c7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'Teagan Maddux',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595255261367-3911c2cf65cd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=690&q=80',
            author: 'Parker Coffman',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595271676080-98d1df02f71f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'Parker Coffman',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595317428853-7d4b208b7192?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'Trnava University',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
    ]

    const imagesRight = [
        { 
            url: 'https://images.unsplash.com/photo-1595088402198-24d44e48d57c?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1254&q=80',
            author: 'Trnava University',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595156066164-410d89ad9a4f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'Trnava University',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595303526913-c7037797ebe7?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1602&q=80',
            author: 'Trnava University',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595239541400-63a8eb5b3c24?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=668&q=80',
            author: 'Trnava University',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },
        { 
            url: 'https://images.unsplash.com/photo-1595245761073-0eb3ca3f179c?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=674&q=80',
            author: 'Trnava University',
            avatar: 'https://images.unsplash.com/photo-1531860494978-9326a0388ef4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=300&q=80',
        },

    ]
</script>


<div class="flex flex-col font-medium text-sm text-gray-600">
    <div>
        <div class="flex px-4 py-3">
            <svg class="w-8 h-8" viewBox="0 0 32 32" aria-labelledby="unsplash-home" aria-hidden="false"><title id="unsplash-home">Unsplash Home</title><path d="M10 9V0h12v9H10zm12 5h10v18H0V14h10v9h12v-9z"></path></svg> 
            <div class="flex flex-1 items-center ml-4 px-3 py-2 rounded-full text-sm font-normal bg-gray-200">
                <svg class="w-4 h-4" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
                <div class="ml-3">Search photos</div>
            </div>
            <div class="flex items-center ml-12 space-x-6">
                <a href="/" class="hover:text-gray-800">Topics</a>
                <a href="/" class="hover:text-gray-800">Explore</a>
                <a href="/" class="hover:text-gray-800">
                    <svg class="w-6 h-6" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z"/></svg>
                </a>
                <a href="/" class="px-3 py-1 rounded border border-gray-400 hover:border-gray-600">Submit a photo</a>
                <a href="/" class="pl-6 py-1 border-l border-gray-500 hover:text-gray-800">Login</a>
                <a href="/" class="px-3 py-1 rounded border border-transparent text-white bg-green-500 hover:bg-green-600">Join free</a>
            </div>
        </div>
        <div class="flex px-4 mt-1 space-x-10 shadow-md">
            <div>
                <a href="/" class="block pb-4 pt-3 border-b-2 border-gray-800 text-gray-800">Editorial</a>
            </div>
            <div class="relative">
                <div class="absolute top-0 text-xs uppercase tracking-wide font-light" style="font-size:0.6rem">Featured</div>
                <a href="/" class="block pb-4 pt-3 border-b-2 border-transparent">
                    Sustainability
                </a>
            </div>
            <a href="/" class="block pb-4 pt-3 border-b-2 border-transparent">
                Wallpapers
            </a>
            <a href="/" class="block pb-4 pt-3 border-b-2 border-transparent">
                COVID-19
            </a>
            <a href="/" class="block pb-4 pt-3 border-b-2 border-transparent">
                Travel
            </a>
            <a href="/" class="block pb-4 pt-3 border-b-2 border-transparent">
                Nature
            </a>
        </div>
    </div>

    <div class="relative flex flex-col" style="background-image:url(https://images.unsplash.com/photo-1569875949045-767b9dd8f916?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&dpr=1&auto=format%2Ccompress&fit=crop&w=1399&h=594)">
        <div class="absolute inset-0 bg-opacity-50 bg-black" />
        <div class="relative container mx-auto pt-32 pb-32">
            <h1 class="text-5xl font-bold text-white">Unsplash</h1>
            <div class="mt-2 font-normal text-lg text-white">
                The internet’s source of <a href="/" class="underline text-gray-300 hover:text-white">freely-usable</a> images.<br />
                Powered by creators everywhere.
            </div>
            <div class="flex items-center w-full py-4 px-4 mt-5 rounded font-normal bg-white">
                <svg class="w-5 h-5" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
                <div class="ml-3">Search free high-resolution photos</div>
            </div>
            <div class="mt-4 font-normal text-white">
                Trending:
                <a href="/" class="text-gray-100 hover:text-white">freely-usable</a>, 
                <a href="/" class="text-gray-100 hover:text-white">wallpapers</a>, 
                <a href="/" class="text-gray-100 hover:text-white">backgrounds</a>, 
                <a href="/" class="text-gray-100 hover:text-white">happy</a>, 
                <a href="/" class="text-gray-100 hover:text-white">love</a>
            </div>
        </div>

        <div class="relative flex items-end justify-between px-3 pb-4 text-gray-400 text-xs">
            <div>
                <a href="/" class="text-white">Photo of the Day</a> by <a href="/" class="text-white">Filip Urban</a>
            </div>
            <div>
                Read more about the <a href="/" class="text-white">Unsplash License</a>
            </div>
            <div class="text-right">
                <img class="inline-block h-6" src="squarespace.png" alt="">
                <div class="mt-1">All you need to create a website.</div>
            </div>
        </div>
    </div>

    <div class="flex pt-8 px-3 space-x-5">
        <div class="w-1/3">
            {#each imagesLeft as image}
                <div class="py-3">
                    <Image {image} />
                </div>
            {/each}
        </div>
        <div class="w-1/3">
            {#each imagesCenter as image}
                <div class="py-3">
                    <Image {image} />
                </div>
            {/each}
        </div>
        <div class="w-1/3">
            {#each imagesRight as image}
                <div class="py-3">
                    <Image {image} />
                </div>
            {/each}
        </div>
    </div>

</div>