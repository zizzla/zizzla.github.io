---
layout: base
title: Zizzla
permalink: /
published: true
---

<div class="flex flex-col">

    <div class="relative visible md:invisible">
        <div class="relative"><span>
            <img src="{{site.baseurl}}/assets/img/jonglering.jpeg" class="absolute w-75 rotate-14 opacity-25 inset-x-0 shadow-xl bg-white w-1/2 mx-auto rounded">
        </span></div>
    </div>

    <div class="flex flex-row-reverse">

        <div class="relative invisible md:visible w-0 md:w-96"><span></span>
            <div class="relative pt-5 me-5"><span>
                <img src="{{site.baseurl}}/assets/img/jonglering.jpeg" class="absolute rotate-14 shadow-xl bg-white mx-auto rounded">
            </span></div>
        </div>

        <!-- <div class="col-12 col-md-8"> -->
        <div class="relative pt-4 w-full "><span>
            <h3 class="justify-start text-4xl">Jonglerar du <strong>säker drift</strong> med krav på <strong>högre avkastning</strong>?</h3>
            <h4 class="text-2xl font-light">Det behöver inte vara så svårt.</h4>
        </span></div>
        <!-- </div> -->
    </div>

    <div class="flex flex-row-reverse pt-20">

        <div class="relative invisible md:visible w-0 md:w-96"><span></span>
            <div class="relative pt-5 me-3"><span>
                <img src="{{site.baseurl}}/assets/img/glada_bollar.png" class="absolute rotate-5 shadow-xl bg-white mx-auto rounded">
            </span></div>
        </div>

        <!-- <div class="col-11 col-md-8"> -->
        <div class="relative pt-4 w-full"><span>
            <h3 class="text-4xl">Vill du <strong>köra hållbart</strong> och samtidigt pricka <strong>alla pristoppar</strong>?</h3>
            <h4 class="text-2xl font-light">Zizzla kompromissar, du kontrollerar.</h4>
        </span></div>
        <!-- </div> -->

    </div>
    
    <!-- <div class="flex flex-col relative ">     
    </div> -->
</div>

<div class="flex flex-col mt-16 md:mt-16 text-center">
    <p class="font-display text-base text-slate-900">Våra kunder och partners</p>
    <ul role="list" class="px-3 mt-4 flex items-center justify-center gap-x-8 sm:flex-col sm:gap-x-0 sm:gap-y-10 xl:flex-row xl:gap-x-12 xl:gap-y-0">
        <li>
            <ul role="list" class="flex flex-col items-center gap-y-8 sm:flex-row sm:gap-x-12 sm:gap-y-0 px-0">
                <li><img alt="Tranås energi" style="color:transparent" src="{{site.baseurl}}/assets/img/logo_tranasenergi.png" class="w-36 drop-shadow-xl/25"></li>
                <li><img alt="Njudung energi" src="{{site.baseurl}}/assets/img/logo_njudung.svg" class="w-36 drop-shadow-xl/25"></li>
                <li><img alt="Nässjö energi" src="{{site.baseurl}}/assets/img/logo_nassjo.svg" class="w-36 drop-shadow-xl/25"></li>
            </ul>
        </li>
        <li>
            <ul role="list" class="flex flex-col items-center gap-y-8 sm:flex-row sm:gap-x-12 sm:gap-y-0 px-0">
                <li><img alt="Vimmerby energi och miljö" src="{{site.baseurl}}/assets/img/logo_vimmerby.svg" class="w-36 drop-shadow-xl/25"></li>
                <li><img alt="Eksjö energi" src="{{site.baseurl}}/assets/img/logo_eksjo.svg" class="w-36 drop-shadow-xl/25"></li>
            </ul>
        </li>
        <li>
            <ul role="list" class="flex flex-col items-center gap-y-8 sm:flex-row sm:gap-x-12 sm:gap-y-0 px-0">
                <li><img alt="Adven" src="{{site.baseurl}}/assets/img/logo_adven.svg" class="w-36 drop-shadow-xl/25"></li>
                <li><img alt="Novotek" src="{{site.baseurl}}/assets/img/logo_novotek.svg" class="w-36 drop-shadow-xl/25"></li>
                <li><img alt="Almi" src="{{site.baseurl}}/assets/img/logo_almi.svg" class="w-36 drop-shadow-xl/25"></li>
            </ul>
        </li>
    </ul>
</div>

<div class="mt-10 grid gap-4 sm:mt-16 lg:grid-cols-3 lg:grid-rows-2">

<!-- <div class="flex flex-row">
    <div class="mx-auto max-w-7xl lg:px-2">
        <div class="mx-auto mt-10 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 border-t border-gray-200 pt-10 sm:mt-16 sm:pt-16 lg:mx-0 lg:max-w-none lg:grid-cols-3"> -->
        
            {% if site.paginate %}
                {% assign posts = paginator.posts %}
            {% else %}
                {% assign posts = site.posts %}
            {% endif %}

            {%- include post-items.html posts = posts %}
            
        <!-- </div>
    </div> -->
</div>
