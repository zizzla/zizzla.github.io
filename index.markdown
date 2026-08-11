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

<section class="w-full bg-navy py-16 sm:py-20" aria-labelledby="services-workflow-heading" data-services-workflow>
    <div class="mx-auto max-w-9xl px-6">
        <div class="max-w-2xl">
            <h2 id="services-workflow-heading" class="text-3xl font-bold text-white sm:text-4xl">Så fungerar Zizzla</h2>
            <p class="mt-4 text-base leading-7 text-white/60">Från prognos till fysisk aktivering – i ett sammanhängande arbetsflöde.</p>
        </div>

        <div class="mt-10 grid gap-4 sm:grid-cols-2 lg:grid-cols-4" role="tablist" aria-label="Zizzlas arbetsflöde">
            <button type="button" id="services-tab-planera" role="tab" aria-selected="true" aria-controls="services-panel-planera" data-services-tab="planera" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-spring bg-white/5 p-6 text-left transition duration-300 aria-selected:border-spring aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-spring lg:hover:-translate-y-1 lg:hover:border-spring/50">
                <img src="{{ site.baseurl }}/assets/img/services/PLANERA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-spring">Steg 1</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Planera</h3>
                    <p class="mt-3 text-sm leading-6 text-white/60">Prognostisera last och marknadspriser. Optimera produktionen utifrån fysisk verklighet, tillgänglighet och tillfälliga begränsningar.</p>
                    <p class="mt-4 text-xs font-semibold text-spring opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Prognos → Begränsningar → Optimal plan</p>
                </div>
            </button>

            <button type="button" id="services-tab-besluta" role="tab" aria-selected="false" aria-controls="services-panel-besluta" data-services-tab="besluta" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-yellow bg-white/5 p-6 text-left transition duration-300 aria-selected:border-yellow aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-yellow lg:hover:-translate-y-1 lg:hover:border-yellow/50">
                <img src="{{ site.baseurl }}/assets/img/services/BESLUTA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-yellow">Steg 2</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Besluta</h3>
                    <p class="mt-3 text-sm leading-6 text-white/60">Välj marknad, resurs och pris – manuellt, med beslutsstöd eller helt automatiserat. Driftvillkoren följer alltid med.</p>
                    <p class="mt-4 text-xs font-semibold text-yellow opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Manuellt → Beslutsstöd → Automatiskt</p>
                </div>
            </button>

            <button type="button" id="services-tab-aktivera" role="tab" aria-selected="false" aria-controls="services-panel-aktivera" data-services-tab="aktivera" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-pink bg-white/5 p-6 text-left transition duration-300 aria-selected:border-pink aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-pink lg:hover:-translate-y-1 lg:hover:border-pink/50">
                <img src="{{ site.baseurl }}/assets/img/services/AKTIVERA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-pink">Steg 3</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Aktivera</h3>
                    <p class="mt-3 text-sm leading-6 text-white/60">Schemalägg och styr resurser, följ aktiveringar och hantera avvikelser – manuellt, halvautomatiskt eller automatiskt.</p>
                    <p class="mt-4 text-xs font-semibold text-pink opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Schemalägg → Aktivera → Följ upp</p>
                </div>
            </button>

            <button type="button" id="services-tab-visualisera" role="tab" aria-selected="false" aria-controls="services-panel-visualisera" data-services-tab="visualisera" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-purple bg-white/5 p-6 text-left transition duration-300 aria-selected:border-purple aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-purple lg:hover:-translate-y-1 lg:hover:border-purple/50">
                <img src="{{ site.baseurl }}/assets/img/services/VISUALISERA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-purple">Steg 4</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Visualisera</h3>
                    <p class="mt-3 text-sm leading-6 text-white/60">Samla prognoser, marknad, produktion och drift i en gemensam lägesbild – från plan till faktiskt utfall.</p>
                    <p class="mt-4 text-xs font-semibold text-purple opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Plan → Drift → Utfall</p>
                </div>
            </button>
        </div>

        <div class="mt-6">
            <div id="services-panel-planera" role="tabpanel" aria-labelledby="services-tab-planera" data-services-panel="planera" class="rounded-2xl border border-white/10 border-l-4 border-l-spring bg-white/5 p-6">
                <div class="grid gap-6 md:grid-cols-2 md:gap-10">
                    <div>
                        <h3 class="text-xl font-bold text-white">Planera med verkligheten som begränsning</h3>
                        <p class="mt-3 text-sm leading-6 text-white/70">Zizzla kombinerar prognoser för last, priser och andra relevanta signaler med anläggningens faktiska möjligheter. Optimeringen tar hänsyn till både permanenta och tillfälliga begränsningar.</p>
                    </div>
                    <div>
                        <p class="text-xs font-bold uppercase tracking-widest text-spring">Det här händer</p>
                        <ul class="mt-3 space-y-2 text-sm text-white/70">
                            <li>Prognoser för last och marknad</li>
                            <li>Fysiska och tillfälliga begränsningar</li>
                            <li>Optimal körplan över flera marknader</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div id="services-panel-besluta" role="tabpanel" aria-labelledby="services-tab-besluta" data-services-panel="besluta" class="rounded-2xl border border-white/10 border-l-4 border-l-yellow bg-white/5 p-6" hidden>
                <div class="grid gap-6 md:grid-cols-2 md:gap-10">
                    <div>
                        <h3 class="text-xl font-bold text-white">Välj hur mycket ni vill automatisera</h3>
                        <p class="mt-3 text-sm leading-6 text-white/70">Marknads- och driftbeslut kan tas manuellt, med beslutsstöd eller helt algoritmiskt. Ni kan börja försiktigt och automatisera mer när organisationen är redo.</p>
                    </div>
                    <div>
                        <p class="text-xs font-bold uppercase tracking-widest text-yellow">Det här händer</p>
                        <ul class="mt-3 space-y-2 text-sm text-white/70">
                            <li>Manuell trading</li>
                            <li>Semi-automatisk trading</li>
                            <li>Fullt algoritmisk trading</li>
                        </ul>
                        <div class="mt-5">
                            {% if site.zizzla.demo_form_url and site.zizzla.demo_form_url != "" %}
                            <a class="inline-flex items-center rounded-full border border-yellow/60 px-5 py-2 text-sm font-bold text-white transition hover:border-yellow" href="{{ site.zizzla.demo_form_url }}" target="_blank" rel="noopener">
                            {% else %}
                            <a class="inline-flex items-center rounded-full border border-yellow/60 px-5 py-2 text-sm font-bold text-white transition hover:border-yellow" href="mailto:nyfiken@zizzla.com?subject=Demo%20av%20Zizzla">
                            {% endif %}
                                Boka demo
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <div id="services-panel-aktivera" role="tabpanel" aria-labelledby="services-tab-aktivera" data-services-panel="aktivera" class="rounded-2xl border border-white/10 border-l-4 border-l-pink bg-white/5 p-6" hidden>
                <div class="grid gap-6 md:grid-cols-2 md:gap-10">
                    <div>
                        <h3 class="text-xl font-bold text-white">Från beslut till fysisk drift</h3>
                        <p class="mt-3 text-sm leading-6 text-white/70">Zizzla kan schemalägga och styra resurser när marknadsbeslut ska omsättas i faktisk drift. Aktivering kan ske manuellt, halvautomatiskt eller automatiskt.</p>
                    </div>
                    <div>
                        <p class="text-xs font-bold uppercase tracking-widest text-pink">Det här händer</p>
                        <ul class="mt-3 space-y-2 text-sm text-white/70">
                            <li>Schemalägg resurser</li>
                            <li>Följ aktiveringar och avvikelser</li>
                            <li>Manuell, halvautomatisk eller automatisk aktivering</li>
                        </ul>
                        <div class="mt-5">
                            {% if site.zizzla.demo_form_url and site.zizzla.demo_form_url != "" %}
                            <a class="inline-flex items-center rounded-full border border-pink/60 px-5 py-2 text-sm font-bold text-white transition hover:border-pink" href="{{ site.zizzla.demo_form_url }}" target="_blank" rel="noopener">
                            {% else %}
                            <a class="inline-flex items-center rounded-full border border-pink/60 px-5 py-2 text-sm font-bold text-white transition hover:border-pink" href="mailto:nyfiken@zizzla.com?subject=Demo%20av%20Zizzla">
                            {% endif %}
                                Boka demo
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <div id="services-panel-visualisera" role="tabpanel" aria-labelledby="services-tab-visualisera" data-services-panel="visualisera" class="rounded-2xl border border-white/10 border-l-4 border-l-purple bg-white/5 p-6" hidden>
                <div class="grid gap-6 md:grid-cols-2 md:gap-10">
                    <div>
                        <h3 class="text-xl font-bold text-white">Se hela kedjan i samma lägesbild</h3>
                        <p class="mt-3 text-sm leading-6 text-white/70">Prognoser, marknad, körplan, bud, aktivering och faktiskt utfall kan följas i samma sammanhang. Det ger både operativ överblick och bättre återkoppling över tid.</p>
                    </div>
                    <div>
                        <p class="text-xs font-bold uppercase tracking-widest text-purple">Det här händer</p>
                        <ul class="mt-3 space-y-2 text-sm text-white/70">
                            <li>Plan och bud</li>
                            <li>Drift och aktivering</li>
                            <li>Utfall och uppföljning</li>
                        </ul>
                    </div>
                </div>
            </div>

            <div data-services-hover-preview="besluta" class="rounded-2xl border border-white/10 border-l-4 border-l-yellow bg-white/5 p-6" hidden>
                <div class="grid gap-6 lg:grid-cols-3 lg:items-center lg:gap-10">
                    <div class="overflow-hidden rounded-xl border border-white/10 bg-navy p-2 lg:col-span-2">
                        <img src="{{ site.baseurl }}/assets/video/besluta-da.gif" alt="Budläggning i Zizzla Planner" class="max-h-72 w-full object-contain" data-services-preview-image>
                    </div>
                    <div>
                        <p class="text-xs font-bold uppercase tracking-widest text-yellow">Day-ahead / marknadsbud</p>
                        <h3 class="mt-3 text-xl font-bold text-white">Budläggning i Zizzla Planner</h3>
                        <p class="mt-3 text-sm leading-6 text-white/70">Från körplan till marknadsbud i samma arbetsflöde.</p>
                    </div>
                </div>
            </div>
        </div>

        <div class="mt-8">
            <a href="{{ site.baseurl }}/services/" class="inline-flex items-center rounded-full border border-white/30 px-6 py-3 text-sm font-bold text-white">Utforska tjänster</a>
        </div>
    </div>
</section>

<script>
    (() => {
        const workflow = document.querySelector("[data-services-workflow]");
        if (!workflow) return;

        const tabs = workflow.querySelectorAll("[data-services-tab]");
        const panels = workflow.querySelectorAll("[data-services-panel]");
        const decideTab = workflow.querySelector('[data-services-tab="besluta"]');
        const hoverPreview = workflow.querySelector('[data-services-hover-preview="besluta"]');
        const previewImage = workflow.querySelector("[data-services-preview-image]");
        const desktop = window.matchMedia("(min-width: 1024px)");
        let previewAvailable = previewImage.complete && previewImage.naturalWidth > 0;
        let previewActive = false;

        const selectedStep = () =>
            workflow.querySelector('[data-services-tab][aria-selected="true"]')?.dataset.servicesTab;

        const showSelectedPanel = () => {
            previewActive = false;
            hoverPreview.hidden = true;

            panels.forEach((panel) => {
                panel.hidden = panel.dataset.servicesPanel !== selectedStep();
            });
        };

        const showHoverPreview = () => {
            if (!desktop.matches || !previewAvailable) return;

            previewActive = true;
            panels.forEach((panel) => {
                panel.hidden = true;
            });
            hoverPreview.hidden = false;
        };

        previewImage.addEventListener("load", () => {
            previewAvailable = true;
        });

        previewImage.addEventListener("error", () => {
            previewAvailable = false;
            if (previewActive) showSelectedPanel();
        });

        decideTab.addEventListener("mouseenter", showHoverPreview);
        decideTab.addEventListener("mouseleave", () => {
            if (previewActive) showSelectedPanel();
        });

        desktop.addEventListener("change", () => {
            if (!desktop.matches && previewActive) showSelectedPanel();
        });

        tabs.forEach((tab) => {
            tab.addEventListener("click", () => {
                tabs.forEach((item) => {
                    item.setAttribute("aria-selected", String(item === tab));
                });

                if (!previewActive) showSelectedPanel();
            });
        });
    })();
</script>

<div class="mx-auto mt-10 max-w-9xl px-6 sm:mt-16">
    <div class="max-w-2xl">
        <h2 class="text-3xl font-bold text-white sm:text-4xl">Insikter</h2>
        <p class="mt-4 text-base leading-7 text-white/60">Analyser och perspektiv på energimarknaden, flexibilitet och framtidens drift.</p>
    </div>
</div>

<div class="mx-auto mt-8 grid max-w-9xl gap-4 px-6 lg:grid-cols-3 lg:grid-rows-2">
<!-- <div class="flex flex-row">
    <div class="mx-auto max-w-7xl lg:px-2">
        <div class="mx-auto mt-10 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 border-t border-gray-200 pt-10 sm:mt-16 sm:pt-16 lg:mx-0 lg:max-w-none lg:grid-cols-3"> -->
        
            {% assign posts = site.posts | slice: 0, 3 %}

            {%- include post-items.html posts = posts %}
            
        <!-- </div>
    </div> -->
</div>

<div class="mx-auto mt-8 flex max-w-9xl justify-end px-6">
    <a href="{{ '/blogg/' | relative_url }}" class="text-sm font-bold text-spring transition hover:text-white">
        Fler artiklar →
    </a>
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
                    {% if site.zizzla.demo_form_url and site.zizzla.demo_form_url != "" %}
                    <a class="group inline-flex items-center gap-2 rounded-full bg-spring px-6 py-3 text-sm font-bold text-navy hover:opacity-90 transition" href="{{ site.zizzla.demo_form_url }}" target="_blank" rel="noopener">
                    {% else %}
                    <a class="group inline-flex items-center gap-2 rounded-full bg-spring px-6 py-3 text-sm font-bold text-navy hover:opacity-90 transition" href="mailto:nyfiken@zizzla.com?subject=Demo%20av%20Zizzla">
                    {% endif %}
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
