---
layout: base
title: Zizzla
permalink: /
published: true
---

<div class="relative min-h-screen bg-navy flex flex-col">
    <section class="relative pt-46 flex flex-col min-h-screen overflow-hidden">
    
        <div class="absolute inset-0 pointer-events-none flex justify-center">
            <div class="relative w-full max-w-9xl h-full">
                
                <div class="absolute inset-0 z-0">
                    <img src="{{site.baseurl}}/assets/img/alex_octopus.png" 
                        class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 min-h-full max-w-full object-cover opacity-100">
                </div>

                <div class="absolute inset-0 z-10 mix-blend-overlay opacity-100">
                    <svg width="100%" height="100%" preserveAspectRatio="xMidYMid slice" xmlns="http://www.w3.org/2000/svg" class="w-full h-full">
                        <filter id="seamless-stir" x="-20%" y="-20%" width="140%" height="140%">
                            <feTurbulence type="fractalNoise" baseFrequency="0.01 0.015" numOctaves="3" result="noise1">
                                <animate attributeName="baseFrequency" values="0.01 0.015; 0.016 0.022; 0.01 0.015" dur="35s" repeatCount="indefinite" calcMode="spline" keyTimes="0; 0.4; 1" keySplines="0.42 0 0.58 1; 0.42 0 0.58 1" />
                            </feTurbulence>
                            <feTurbulence type="fractalNoise" baseFrequency="0.02 0.01" numOctaves="3" result="noise2">
                                <animate attributeName="baseFrequency" values="0.02 0.01; 0.012 0.018; 0.02 0.01" dur="23s" repeatCount="indefinite" calcMode="spline" keyTimes="0; 0.65; 1" keySplines="0.33 0 0.67 1; 0.33 0 0.67 1" />
                            </feTurbulence>
                            <feComposite in="noise1" in2="noise2" operator="arithmetic" k1="0.5" k2="0.5" k3="0" k4="0" result="mixedNoise" />
                            <feSpecularLighting in="mixedNoise" specularExponent="35" lighting-color="#e0f7fa" result="light">
                                <feDistantLight azimuth="225" elevation="60" />
                            </feSpecularLighting>
                            <feDisplacementMap in="SourceGraphic" in2="mixedNoise" scale="45" xChannelSelector="R" yChannelSelector="G" result="distorted" />
                            <feComposite in="light" in2="distorted" operator="arithmetic" k1="0.6" k2="1" k3="0.1" k4="0" />
                        </filter>
                        <rect width="100%" height="100%" fill="#001233" filter="url(#seamless-stir)" />
                    </svg>
                </div>
            </div>
        </div>

        <div class="relative z-20 flex-grow flex items-center justify-center text-center px-6 pb-20">
            <div class="max-w-5xl mx-auto">
                <h1 class="text-5xl md:text-6xl font-black leading-[1.1] tracking-normal text-white mb-10">
                    Jonglerar du <span class="text-white">säker drift</span> <br>
                    med krav på <span class="text-white">högre avkastning</span>?
                </h1>
                <div class="space-y-6 mb-12">
                    <p class="text-2xl md:text-3xl font-bold tracking-wide text-white">Det behöver inte vara så svårt.</p>
                    <p class="text-lg md:text-xl font-light tracking-wide text-white/80 max-w-2xl mx-auto">Med <span class="text-spring">Zizzla</span> får du ett optimalt körschema för varje situation och marknad.</p>
                </div>
                <!-- <a href="#nyfiken" class="inline-block px-12 py-5 bg-spring text-navy font-black text-xl uppercase tracking-widest rounded-full hover:scale-105 transition-transform">Nyfiken?</a> -->
            </div>
        </div>

        <div class="relative z-20 w-full py-12 bg-navy/0 overflow-hidden">
            <div class="max-w-9xl mx-auto px-0">
                <p class="text-center text-[10px] uppercase tracking-[0.4em] text-white/40 mb-10">Våra kunder och partners</p>
                
                <div class="relative flex overflow-hidden">
                    <div class="animate-scroll flex items-center space-x-24 pr-24">
                        {% assign logo_style = "h-8 w-auto opacity-60 hover:opacity-100 transition-opacity brightness-0 invert flex-shrink-0" %}
                        
                        <img alt="Adven" src="{{site.baseurl}}/assets/img/logo_adven.svg" class="{{ logo_style }}">
                        <img alt="Novotek" src="{{site.baseurl}}/assets/img/logo_novotek.svg" class="{{ logo_style }}">
                        <img alt="Nässjö energi" src="{{site.baseurl}}/assets/img/logo_nassjo.svg" class="{{ logo_style }}">
                        <img alt="Almi" src="{{site.baseurl}}/assets/img/logo_almi.svg" class="{{ logo_style }}">
                        <img alt="Tranås energi" src="{{site.baseurl}}/assets/img/logo_tranasenergi.png" class="{{ logo_style }}">
                        <img alt="Energimyndigheten" src="{{site.baseurl}}/assets/img/logo_energimyndigheten.svg" class="{{ logo_style }}">
                        <img alt="Inclusive Business Partners" src="{{site.baseurl}}/assets/img/logo_inclusive_business.png" class="{{ logo_style }}">


                        <img alt="Adven" src="{{site.baseurl}}/assets/img/logo_adven.svg" class="{{ logo_style }}">
                        <img alt="Novotek" src="{{site.baseurl}}/assets/img/logo_novotek.svg" class="{{ logo_style }}">
                        <img alt="Nässjö energi" src="{{site.baseurl}}/assets/img/logo_nassjo.svg" class="{{ logo_style }}">
                        <img alt="Almi" src="{{site.baseurl}}/assets/img/logo_almi.svg" class="{{ logo_style }}">
                        <img alt="Tranås energi" src="{{site.baseurl}}/assets/img/logo_tranasenergi.png" class="{{ logo_style }}">
                        <img alt="Energimyndigheten" src="{{site.baseurl}}/assets/img/logo_energimyndigheten.svg" class="{{ logo_style }}">
                        <img alt="Inclusive Business Partners" src="{{site.baseurl}}/assets/img/logo_inclusive_business.png" class="{{ logo_style }}">

                    </div>
                </div>
            </div>
        </div>
    </section>
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

<section class="w-full border-t border-white/10">
    <div class="mx-auto max-w-screen-2xl px-8 py-16">
        <div class="grid gap-10 lg:grid-cols-2 lg:items-center">
            <div>
                <h2 class="text-3xl font-bold text-white">
                    Vill du se hur Zizzla fungerar i praktiken?
                </h2>
                <p class="mt-4 text-sm leading-6 text-white/60">
                    Boka en kort demo så visar vi hur ni kan gå från prognos till körplan, bud och aktivering i ett enkelt arbetsflöde.
                </p>
                <div class="mt-6">
                    <a class="group inline-flex items-center gap-2 rounded-full bg-spring px-6 py-3 text-sm font-bold text-navy hover:opacity-90 transition" href="mailto:nyfiken@zizzla.com?subject=Demo%20av%20Zizzla">
                        Boka demo
                        <span class="transition duration-300 group-hover:translate-x-1">→</span>
                    </a>
                </div>
            </div>

            <div tabindex="0" class="group rounded-lg border border-white/10 bg-white/5 p-6 transition duration-300 hover:-translate-y-1 hover:border-spring/50 focus:outline-none focus:border-spring/50">
                <div class="flex items-center justify-between gap-4">
                    <div>
                        <p class="text-sm font-bold text-white">Zizzla Planner</p>
                        <p class="mt-1 text-sm text-white/50">Budförslag redo</p>
                    </div>
                    <span class="rounded-full bg-white/10 px-3 py-1 text-sm text-white/60 transition duration-300 group-hover:bg-spring group-hover:text-navy group-focus:bg-spring group-focus:text-navy">
                        <span class="group-hover:hidden group-focus:hidden">Skicka</span>
                        <span class="hidden group-hover:inline group-focus:inline">Skickat</span>
                    </span>
                </div>

                <svg class="mt-6 h-16 w-full opacity-70 transition duration-300 group-hover:opacity-100" viewBox="0 0 320 80" role="img" aria-label="Elplan, prisprognos och mFRR ned-bud">
                    <path d="M16 48 H304" fill="none" class="stroke-spring" stroke-width="4" stroke-linecap="round" />
                    <path d="M16 58 C64 54 96 56 128 46 S176 18 208 28 S260 50 304 42" fill="none" class="stroke-pink opacity-70 transition duration-300 group-hover:opacity-100 group-focus:opacity-100" stroke-width="3" stroke-linecap="round" />
                    <path d="M142 48 C156 50 170 50 184 48 L184 64 C170 68 156 68 142 64 Z" class="fill-spring/10 stroke-spring/60 group-hover:hidden group-focus:hidden" stroke-width="2" stroke-dasharray="4 4" />
                    <path d="M142 48 C156 50 170 50 184 48 L184 64 C170 68 156 68 142 64 Z" class="hidden fill-spring/30 stroke-spring group-hover:block group-focus:block" stroke-width="2" />
                    <circle cx="164" cy="48" r="4" class="fill-spring transition duration-300 group-hover:fill-white group-focus:fill-white" />
                </svg>

                <div class="mt-6 grid gap-3 text-sm">
                    <div class="grid grid-cols-2 gap-3">
                        <div class="rounded bg-spring/10 p-3">
                            <p class="text-white/50">Resurs</p>
                            <p class="mt-1 font-bold text-white">Elpanna</p>
                            <div class="mt-2 flex items-center gap-2 text-xs text-white/60">
                                <span class="h-2 w-2 rounded-full bg-spring"></span>
                                <span>I drift</span>
                            </div>
                            <div class="mt-2 h-2 rounded-full bg-white/10">
                                <div class="h-2 w-1/4 rounded-full bg-spring"></div>
                            </div>
                            <div class="mt-1 flex justify-between gap-2 text-xs text-white/50">
                                <span>1 MW nu</span>
                                <span>+10 MW tillgängligt</span>
                            </div>
                        </div>
                        <div class="rounded bg-white/10 p-3">
                            <p class="text-white/50">Marknad</p>
                            <p class="mt-1 font-bold text-white">mFRR ned</p>
                        </div>
                    </div>

                    <div class="grid grid-cols-2 gap-3">
                        <div class="rounded bg-white/10 p-3">
                            <p class="text-white/50">Budvolym</p>
                            <p class="mt-1 font-bold text-white">4 MW</p>
                        </div>
                        <div class="rounded bg-white/10 p-3">
                            <p class="text-white/50">Pris</p>
                            <p class="mt-1 font-bold text-white">Auto</p>
                        </div>
                    </div>
                </div>

                <div class="mt-6">
                    <div class="h-2 rounded-full bg-white/10">
                        <div class="h-2 w-2/3 rounded-full bg-white/40 transition-all duration-300 group-hover:w-full group-hover:bg-spring group-focus:w-full group-focus:bg-spring"></div>
                    </div>
                    <div class="mt-4 rounded bg-white/10 p-3 transition duration-300 group-hover:bg-spring/20 group-focus:bg-spring/20">
                        <p class="text-sm font-bold text-white transition duration-300 group-hover:text-spring group-focus:text-spring">
                            <span class="group-hover:hidden group-focus:hidden">Bud redo att skickas</span>
                            <span class="hidden group-hover:inline group-focus:inline">Bud skickat till marknad</span>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
