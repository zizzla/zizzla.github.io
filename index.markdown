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
                    <div class="animate-scroll">
                        {% assign logo_style = "h-8 w-auto opacity-60 hover:opacity-100 transition-opacity brightness-0 invert shrink-0" %}
                        {% for copy in (1..2) %}
                        <div class="logo-set"{% if copy == 2 %} aria-hidden="true"{% endif %}>
                            <img alt="{% if copy == 1 %}Adven{% endif %}" src="{{site.baseurl}}/assets/img/logo_adven.svg" width="850" height="200" class="{{ logo_style }}">
                            <img alt="{% if copy == 1 %}Novotek{% endif %}" src="{{site.baseurl}}/assets/img/logo_novotek.svg" width="120" height="32" class="{{ logo_style }}">
                            <img alt="{% if copy == 1 %}Nässjö energi{% endif %}" src="{{site.baseurl}}/assets/img/logo_nassjo.svg" width="522" height="95" class="{{ logo_style }}">
                            <img alt="{% if copy == 1 %}Almi{% endif %}" src="{{site.baseurl}}/assets/img/logo_almi.svg" width="114" height="41" class="{{ logo_style }}">
                            <img alt="{% if copy == 1 %}Tranås energi{% endif %}" src="{{site.baseurl}}/assets/img/logo_tranasenergi.png" width="865" height="429" class="{{ logo_style }}">
                            <img alt="{% if copy == 1 %}Energimyndigheten{% endif %}" src="{{site.baseurl}}/assets/img/logo_energimyndigheten.svg" width="178" height="43" style="aspect-ratio: 177.776 / 42.5197" class="{{ logo_style }}">
                            <img alt="{% if copy == 1 %}Inclusive Business Partners{% endif %}" src="{{site.baseurl}}/assets/img/logo_inclusive_business.png" width="2048" height="459" class="{{ logo_style }}">
                            <!-- Officiella original: https://bixia.se/assets/logos/bixia.svg och https://www.axpo.com/bin/logo-svg (statisk export). -->
                            <img alt="{% if copy == 1 %}Bixia{% endif %}" src="{{site.baseurl}}/assets/img/logo_bixia.svg" width="164" height="52" class="{{ logo_style }}">
                            <img alt="{% if copy == 1 %}Axpo{% endif %}" src="{{site.baseurl}}/assets/img/logo_axpo.svg" width="330" height="130" class="{{ logo_style }}">
                        </div>
                        {% endfor %}
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

        <div class="scroll-mt-24 mt-10 grid grid-cols-2 gap-3 md:gap-4 lg:grid-cols-4" role="tablist" aria-label="Zizzlas arbetsflöde">
            <button type="button" id="services-tab-planera" role="tab" aria-selected="true" aria-controls="services-panel-planera" data-services-tab="planera" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-spring bg-white/5 p-3 md:p-6 text-left transition duration-300 aria-selected:border-spring aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-spring lg:hover:-translate-y-1 lg:hover:border-spring/50">
                <img src="{{ site.baseurl }}/assets/img/services/PLANERA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-spring">Steg 1</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Planera</h3>
                    <p class="hidden md:block mt-3 text-sm leading-6 text-white/60">Prognostisera last och marknadspriser. Optimera produktionen utifrån fysisk verklighet, tillgänglighet och tillfälliga begränsningar.</p>
                    <p class="hidden md:block mt-4 text-xs font-semibold text-spring opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Prognos → Begränsningar → Optimal plan</p>
                </div>
            </button>

            <button type="button" id="services-tab-besluta" role="tab" aria-selected="false" aria-controls="services-panel-besluta" data-services-tab="besluta" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-yellow bg-white/5 p-3 md:p-6 text-left transition duration-300 aria-selected:border-yellow aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-yellow lg:hover:-translate-y-1 lg:hover:border-yellow/50">
                <img src="{{ site.baseurl }}/assets/img/services/BESLUTA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-yellow">Steg 2</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Besluta</h3>
                    <p class="hidden md:block mt-3 text-sm leading-6 text-white/60">Välj marknad, resurs och pris – manuellt, med beslutsstöd eller helt automatiserat. Driftvillkoren följer alltid med.</p>
                    <p class="hidden md:block mt-4 text-xs font-semibold text-yellow opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Manuellt → Beslutsstöd → Automatiskt</p>
                </div>
            </button>

            <button type="button" id="services-tab-aktivera" role="tab" aria-selected="false" aria-controls="services-panel-aktivera" data-services-tab="aktivera" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-pink bg-white/5 p-3 md:p-6 text-left transition duration-300 aria-selected:border-pink aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-pink lg:hover:-translate-y-1 lg:hover:border-pink/50">
                <img src="{{ site.baseurl }}/assets/img/services/AKTIVERA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-pink">Steg 3</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Aktivera</h3>
                    <p class="hidden md:block mt-3 text-sm leading-6 text-white/60">Schemalägg och styr resurser, följ aktiveringar och hantera avvikelser – manuellt, halvautomatiskt eller automatiskt.</p>
                    <p class="hidden md:block mt-4 text-xs font-semibold text-pink opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Schemalägg → Aktivera → Följ upp</p>
                </div>
            </button>

            <button type="button" id="services-tab-visualisera" role="tab" aria-selected="false" aria-controls="services-panel-visualisera" data-services-tab="visualisera" class="group relative overflow-hidden rounded-lg border border-white/10 border-l-4 border-l-purple bg-white/5 p-3 md:p-6 text-left transition duration-300 aria-selected:border-purple aria-selected:bg-white/10 focus:outline-none focus-visible:ring-2 focus-visible:ring-purple lg:hover:-translate-y-1 lg:hover:border-purple/50">
                <img src="{{ site.baseurl }}/assets/img/services/VISUALISERA.svg" alt="" class="absolute inset-0 h-full w-full object-cover opacity-30 transition duration-300 group-aria-selected:opacity-60 lg:group-hover:opacity-60">
                <div class="absolute inset-0 bg-gradient-to-r from-navy/90 via-navy/70 to-navy/30"></div>
                <div class="relative z-10">
                    <p class="text-xs font-bold uppercase tracking-widest text-purple">Steg 4</p>
                    <h3 class="mt-3 text-xl font-bold text-white">Visualisera</h3>
                    <p class="hidden md:block mt-3 text-sm leading-6 text-white/60">Samla prognoser, marknad, produktion och drift i en gemensam lägesbild – från plan till faktiskt utfall.</p>
                    <p class="hidden md:block mt-4 text-xs font-semibold text-purple opacity-60 transition duration-300 lg:opacity-0 lg:group-hover:opacity-100">Plan → Drift → Utfall</p>
                </div>
            </button>
        </div>

        <div class="mt-6">
            <div id="services-panel-planera" role="tabpanel" aria-labelledby="services-tab-planera" tabindex="-1" data-services-panel="planera" class="scroll-mt-24 rounded-2xl border border-white/10 border-l-4 border-l-spring bg-white/5 p-6">
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

            <div id="services-panel-besluta" role="tabpanel" aria-labelledby="services-tab-besluta" tabindex="-1" data-services-panel="besluta" class="scroll-mt-24 rounded-2xl border border-white/10 border-l-4 border-l-yellow bg-white/5 p-6" hidden>
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
                            <a class="inline-flex items-center rounded-full border border-yellow/60 px-5 py-2 text-sm font-bold text-white transition hover:border-yellow" href="mailto:{{ site.email }}" data-contact-open aria-haspopup="dialog" aria-controls="contact-dialog">
                                Nyfiken? Hör av dig.
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <div id="services-panel-aktivera" role="tabpanel" aria-labelledby="services-tab-aktivera" tabindex="-1" data-services-panel="aktivera" class="scroll-mt-24 rounded-2xl border border-white/10 border-l-4 border-l-pink bg-white/5 p-6" hidden>
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
                            <a class="inline-flex items-center rounded-full border border-pink/60 px-5 py-2 text-sm font-bold text-white transition hover:border-pink" href="mailto:{{ site.email }}" data-contact-open aria-haspopup="dialog" aria-controls="contact-dialog">
                                Nyfiken? Hör av dig.
                            </a>
                        </div>
                    </div>
                </div>
            </div>

            <div id="services-panel-visualisera" role="tabpanel" aria-labelledby="services-tab-visualisera" tabindex="-1" data-services-panel="visualisera" class="scroll-mt-24 rounded-2xl border border-white/10 border-l-4 border-l-purple bg-white/5 p-6" hidden>
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

            <div data-services-hover-preview="aktivera" class="scroll-mt-24 rounded-2xl border border-white/10 border-l-4 border-l-pink bg-white/5 p-6" hidden>
                <div class="grid gap-6 lg:grid-cols-3 lg:items-center lg:gap-10">
                    <div class="overflow-hidden rounded-xl border border-white/10 bg-navy p-2 lg:col-span-2">
                        <video class="h-72 w-full object-contain" muted loop playsinline preload="metadata" data-services-preview-media>
                            <source src="{{ site.baseurl }}/assets/video/services/aktivera-mfrr-eam-zizzla-v2.mp4" type="video/mp4">
                        </video>
                    </div>
                    <div>
                        <p class="text-xs font-bold uppercase tracking-widest text-pink">mFRR EAM / aktivering</p>
                        <h3 class="mt-3 text-xl font-bold text-white">Aktivering i verklig drift</h3>
                        <p class="mt-3 text-sm leading-6 text-white/70">Från marknadsbeslut till schemaläggning och fysisk aktivering av resursen.</p>
                    </div>
                </div>
            </div>

            <div data-services-hover-preview="besluta" class="scroll-mt-24 rounded-2xl border border-white/10 border-l-4 border-l-yellow bg-white/5 p-6" hidden>
                <div class="grid gap-6 lg:grid-cols-3 lg:items-center lg:gap-10">
                    <div class="overflow-hidden rounded-xl border border-white/10 bg-navy p-2 lg:col-span-2">
                        <img src="{{ site.baseurl }}/assets/video/besluta-da.gif" alt="Budläggning i Zizzla Planner" class="h-72 w-full object-contain" data-services-preview-media>
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
        const previews = workflow.querySelectorAll("[data-services-hover-preview]");
        const desktop = window.matchMedia("(min-width: 1024px)");
        let activePreview = null;

        const selectedStep = () =>
            workflow.querySelector('[data-services-tab][aria-selected="true"]')?.dataset.servicesTab;

        const stopPreviewMedia = (preview) => {
            const video = preview?.querySelector("video[data-services-preview-media]");
            if (video) video.pause();
        };

        const showSelectedPanel = () => {
            stopPreviewMedia(activePreview);
            activePreview = null;
            previews.forEach((preview) => {
                preview.hidden = true;
            });

            panels.forEach((panel) => {
                panel.hidden = panel.dataset.servicesPanel !== selectedStep();
            });
        };

        const showHoverPreview = (preview) => {
            if (!desktop.matches || preview.dataset.previewUnavailable === "true") return;

            activePreview = preview;
            panels.forEach((panel) => {
                panel.hidden = true;
            });
            previews.forEach((item) => {
                item.hidden = item !== preview;
                if (item !== preview) stopPreviewMedia(item);
            });

            const video = preview.querySelector("video[data-services-preview-media]");
            if (video) {
                video.play().catch(() => {
                    preview.dataset.previewUnavailable = "true";
                    if (activePreview === preview) showSelectedPanel();
                });
            }
        };

        previews.forEach((preview) => {
            const step = preview.dataset.servicesHoverPreview;
            const tab = workflow.querySelector(`[data-services-tab="${step}"]`);
            const media = preview.querySelector("[data-services-preview-media]");
            if (!tab || !media) return;

            media.addEventListener("error", () => {
                preview.dataset.previewUnavailable = "true";
                if (activePreview === preview) showSelectedPanel();
            }, true);

            tab.addEventListener("mouseenter", () => showHoverPreview(preview));
            tab.addEventListener("mouseleave", () => {
                if (activePreview === preview) showSelectedPanel();
            });
        });

        desktop.addEventListener("change", () => {
            if (!desktop.matches && activePreview) showSelectedPanel();
        });

        tabs.forEach((tab) => {
            tab.addEventListener("click", () => {
                tabs.forEach((item) => {
                    item.setAttribute("aria-selected", String(item === tab));
                });

                if (!activePreview) showSelectedPanel();
                if (window.matchMedia('(max-width: 767px)').matches) {
                    // Keep all four choices visible above the selected details.
                    const choices = workflow.querySelector('[role="tablist"]');
                    choices.scrollIntoView({ block: 'start', behavior: 'instant' });
                }
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
                    Berätta vad ni vill åstadkomma så tar vi det därifrån.
                </p>
                <div class="mt-6">
                    <a class="group inline-flex items-center gap-2 rounded-full bg-spring px-6 py-3 text-sm font-bold text-navy hover:opacity-90 transition" href="mailto:{{ site.email }}" data-contact-open aria-haspopup="dialog" aria-controls="contact-dialog">
                        Nyfiken? Hör av dig.
                        <span class="transition duration-300 group-hover:translate-x-1">→</span>
                    </a>
                </div>
            </div>

            <div tabindex="0" data-planner-demo x-data="{ active: false, mobile: window.matchMedia('(max-width: 767px)').matches }"
                 x-on:resize.window="mobile = window.matchMedia('(max-width: 767px)').matches; if (!mobile) active = false"
                 x-bind:data-active="active" x-bind:role="mobile ? 'button' : null" x-bind:aria-pressed="mobile ? active : null"
                 x-on:click="if (mobile) active = !active"
                 x-on:keydown.enter="if (mobile) { $event.preventDefault(); active = !active }"
                 x-on:keydown.space="if (mobile) { $event.preventDefault(); active = !active }"
                 class="group rounded-lg border border-white/10 bg-white/5 p-6 transition duration-300 md:hover:-translate-y-1 md:hover:border-spring/50 focus:outline-none focus:border-spring/50">
                <p class="mb-4 text-sm text-spring md:hidden" x-text="active ? 'Tryck igen för att återställa exemplet' : 'Tryck för att testa budförslaget'">Tryck för att testa budförslaget</p>
                <div class="flex items-center justify-between gap-4">
                    <div>
                        <p class="text-sm font-bold text-white">Zizzla Planner</p>
                        <p class="mt-1 text-sm text-white/50">Budförslag redo</p>
                    </div>
                    <span class="rounded-full bg-white/10 px-3 py-1 text-sm text-white/60 transition duration-300 md:group-hover:bg-spring max-md:group-data-[active=true]:bg-spring md:group-hover:text-navy max-md:group-data-[active=true]:text-navy md:group-focus:bg-spring max-md:group-data-[active=true]:bg-spring md:group-focus:text-navy max-md:group-data-[active=true]:text-navy">
                        <span class="md:group-hover:hidden max-md:group-data-[active=true]:hidden md:group-focus:hidden max-md:group-data-[active=true]:hidden">Skicka</span>
                        <span class="hidden md:group-hover:inline max-md:group-data-[active=true]:inline md:group-focus:inline max-md:group-data-[active=true]:inline">Skickat</span>
                    </span>
                </div>

                <svg class="mt-6 h-16 w-full opacity-70 transition duration-300 md:group-hover:opacity-100 max-md:group-data-[active=true]:opacity-100" viewBox="0 0 320 80" role="img" aria-label="Elplan, prisprognos och mFRR ned-bud">
                    <path d="M16 48 H304" fill="none" class="stroke-spring" stroke-width="4" stroke-linecap="round" />
                    <path d="M16 58 C64 54 96 56 128 46 S176 18 208 28 S260 50 304 42" fill="none" class="stroke-pink opacity-70 transition duration-300 md:group-hover:opacity-100 max-md:group-data-[active=true]:opacity-100 md:group-focus:opacity-100 max-md:group-data-[active=true]:opacity-100" stroke-width="3" stroke-linecap="round" />
                    <path d="M142 48 C156 50 170 50 184 48 L184 64 C170 68 156 68 142 64 Z" class="fill-spring/10 stroke-spring/60 md:group-hover:hidden max-md:group-data-[active=true]:hidden md:group-focus:hidden max-md:group-data-[active=true]:hidden" stroke-width="2" stroke-dasharray="4 4" />
                    <path d="M142 48 C156 50 170 50 184 48 L184 64 C170 68 156 68 142 64 Z" class="hidden fill-spring/30 stroke-spring md:group-hover:block max-md:group-data-[active=true]:block md:group-focus:block max-md:group-data-[active=true]:block" stroke-width="2" />
                    <circle cx="164" cy="48" r="4" class="fill-spring transition duration-300 md:group-hover:fill-white max-md:group-data-[active=true]:fill-white md:group-focus:fill-white max-md:group-data-[active=true]:fill-white" />
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
                        <div class="h-2 w-2/3 rounded-full bg-white/40 transition-all duration-300 md:group-hover:w-full max-md:group-data-[active=true]:w-full md:group-hover:bg-spring max-md:group-data-[active=true]:bg-spring md:group-focus:w-full max-md:group-data-[active=true]:w-full md:group-focus:bg-spring max-md:group-data-[active=true]:bg-spring"></div>
                    </div>
                    <div class="mt-4 rounded bg-white/10 p-3 transition duration-300 md:group-hover:bg-spring/20 max-md:group-data-[active=true]:bg-spring/20 md:group-focus:bg-spring/20 max-md:group-data-[active=true]:bg-spring/20">
                        <p class="text-sm font-bold text-white transition duration-300 md:group-hover:text-spring max-md:group-data-[active=true]:text-spring md:group-focus:text-spring max-md:group-data-[active=true]:text-spring">
                            <span class="md:group-hover:hidden max-md:group-data-[active=true]:hidden md:group-focus:hidden max-md:group-data-[active=true]:hidden">Bud redo att skickas</span>
                            <span class="hidden md:group-hover:inline max-md:group-data-[active=true]:inline md:group-focus:inline max-md:group-data-[active=true]:inline">Bud skickat till marknad</span>
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
