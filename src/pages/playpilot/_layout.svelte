<div class="bg-gray-900">
    <div class="sticky top-0 z-10">
        <div class="flex items-center px-8 py-4 bg-gray-900">
            <div class="flex items-center">
                <img src="playpilot-logo.png" alt="" class="h-10" />
                <img src="playpilot-logo-typography.png" alt="" class="h-6 ml-3" />
            </div>
            <div class="ml-16 flex-1 space-x-16 font-bold text-sm text-white">
                <a href="/">Movies</a>
                <a href="/">Shows</a>
                <a href="/">Kids</a>
                <a href="/">Documentaries</a>
                <a href="/">Cinema</a>
            </div>
            <button class="px-5 py-2 rounded-md font-bold text-xs uppercase text-white bg-red-500 hover:bg-red-400 transition duration-150">Sign in</button>
        </div>
        <div class="flex px-8 py-3 font-semibold text-sm text-gray-500 bg-gray-800">
            <svg class="w-6 h-6" fill="none" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" viewBox="0 0 24 24" stroke="currentColor"><path d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
            <div class="ml-6">
                Search across all streaming services
            </div>
        </div>
    </div>

    <div class="pb-24">
        <slot />
    </div>

    <div class="p-8 bg-gray-800">
        <div class="font-bold uppercase text-white">Om Playpilot</div>
        <div class="mt-2 font-semibold text-xs text-white">
            Hitta enkelt de bästa filmerna och serierna från Netflix, Viaplay, HBO, SVT Play och alla andra streamingtjänster!
            <br/><a class="text-blue-300" href="/">Skapa ett gratiskonto</a> att spara dina tjänster, watchlista filmer och serier du vill se, följ dina vänner och mycket mer!
        </div>
        <div class="mt-8">
            <img class="h-10 inline-block" src="playpilot/appstore-badge.svg" alt="" />
            <img class="h-10 ml-3 inline-block" src="playpilot/google-play-badge.svg" alt="" />
        </div>
        <div class="flex mt-8">
            <div class="w-1/3">
                <h5 class="font-bold text-md uppercase text-white">Topp 5 filmer</h5>
                <ul class="mt-2 space-y-3 font-medium text-xs text-blue-300">
                    <li class="">
                        <a href="/" class="">Jojo Rabbit</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Parasite</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Once Upon a Time... in Hollywood</a>
                    </li>
                    <li class="">
                        <a href="/" class="">1917</a>
                    </li>
                    <li class="">
                        <a href="/" class="">The Old Guard</a>
                    </li>
                </ul>
            </div>
            <div class="w-1/3">
                <h5 class="font-bold text-md uppercase text-white">Topp 5 serier</h5>
                <ul class="mt-2 space-y-3 font-medium text-xs text-blue-300">
                    <li class="">
                        <a href="/" class="">Jojo Rabbit</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Parasite</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Once Upon a Time... in Hollywood</a>
                    </li>
                    <li class="">
                        <a href="/" class="">1917</a>
                    </li>
                    <li class="">
                        <a href="/" class="">The Old Guard</a>
                    </li>
                </ul>
            </div>
            <div class="w-1/3">
                <h5 class="font-bold text-md uppercase text-white">Playpilot</h5>
                <ul class="mt-2 space-y-3 font-medium text-xs text-blue-300">
                    <li class="">
                        <a href="/" class="">Om Playpilot</a>
                    </li>
                    <li class="">
                        <a href="/" class="">FAQ</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Jobb</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Cookiepolicy</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Integritetspolicy</a>
                    </li>
                    <li class="">
                        <a href="/" class="">Användaravtal</a>
                    </li>
                </ul>
            </div>

        </div>

        <div class="mt-10 font-medium text-xs text-gray-300">
            © Playpilot AB (Org nr. 556946-8530), Valhallavägen 66, 114 27 Stockholm, Sverige
        </div>
        <div class="mt-3 font-medium text-xs text-gray-700">
            v2.4.1 (92f1949)
        </div>

        <div class="mt-3 font-medium text-sm text-white">
            <div>
                <img class="inline-block w-8" src="playpilot/se.png" alt="">
                <span class="ml-1">Sverige</span>
            </div>
            <div class="mt-2">
                <img class="inline-block w-8" src="playpilot/se.png" alt="">
                <span class="ml-1">Svenska</span>
            </div>
        </div>
    </div>
</div>