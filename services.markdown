---
layout: base
title: Tjänster
permalink: /services/
published: true
description: Zizzla samlar prognoser, optimering, budgivning, styrning och uppföljning för fjärrvärme och industri.
---

<div class="services-page mx-auto max-w-7xl">
  <section class="grid items-center gap-10 pb-16 pt-32 lg:grid-cols-5 lg:gap-16 lg:pb-24 lg:pt-36" aria-labelledby="services-title">
    <div class="lg:col-span-2">
      <p class="text-xs font-bold uppercase tracking-[0.2em] text-spring">Ett sammanhängande arbetsflöde</p>
      <h1 id="services-title" class="mt-5 text-4xl font-black leading-[1.06] tracking-tight sm:text-5xl xl:text-6xl">Från prognos till automatisk drift</h1>
      <p class="mt-6 max-w-xl text-lg leading-8 text-white/70">Zizzla samlar prognoser, optimering, budgivning, styrning och uppföljning i ett sammanhängande arbetsflöde för fjärrvärme och industri.</p>
      <a href="#zizzla-tjanster" class="mt-8 inline-flex items-center gap-3 rounded-full bg-spring px-6 py-3 font-bold text-navy focus-visible:outline-2 focus-visible:outline-offset-4 focus-visible:outline-spring">Utforska tjänsterna <span aria-hidden="true">↓</span></a>
    </div>
    <figure class="min-w-0 lg:col-span-3">
      <img src="{{ '/assets/img/services/planner-vision.png' | relative_url }}" width="1122" height="1402" alt="Illustrativ produktvy av Zizzla Planner med optimering, portföljgraf, marknadsbud och granskning i samma arbetsyta." class="h-auto w-full rounded-2xl border border-white/15" fetchpriority="high">
      <figcaption class="mt-3 flex flex-wrap justify-between gap-2 text-xs leading-5 text-white/50"><span>Illustrativ produktvy</span><a href="{{ '/assets/img/services/planner-vision.png' | relative_url }}" class="underline underline-offset-4 hover:text-white">Öppna bilden i full storlek</a></figcaption>
    </figure>
  </section>

  <section class="rounded-3xl border border-spring/20 bg-white/[0.025] px-4 py-12 sm:px-8 lg:py-16" aria-labelledby="system-title">
    <div class="mx-auto max-w-2xl text-center">
      <p class="text-xs font-bold uppercase tracking-[0.2em] text-spring">Systemöversikt · Sex delar, ett Zizzla</p>
      <h2 id="system-title" class="mt-4 text-3xl font-bold tracking-tight sm:text-4xl">Allt hänger ihop</h2>
      <p class="mt-5 text-base leading-7 text-white/70">Zizzlas tjänster är inte separata verktyg. Prognoser, optimering, budgivning, styrning, visualisering och uppföljning är delar av samma arbetsflöde.</p>
    </div>
    <p class="mt-6 text-center text-sm text-spring">Välj en form och utforska tjänsten.</p>
    <div class="system-map relative mx-auto mt-8 max-w-4xl">
      <img src="{{ '/assets/img/services/zizzla-services-system.png' | relative_url }}" width="1600" height="1153" alt="Zizzlas samlade formspråk: planering, beslut, styrning och visualisering binds samman med kugghjul och symboler för utveckling och värde." class="h-auto w-full" decoding="async">
      {% for service in site.data.services %}
      <a href="#service-{{ service.id }}" data-system-service="{{ service.id }}" aria-controls="service-{{ service.id }}" aria-label="Utforska {{ service.title | escape }}" class="system-hotspot system-hotspot--{{ service.id }}">
        <span class="system-label"><span aria-hidden="true">0{{ forloop.index }}</span><span class="sr-only sm:not-sr-only"> {{ service.short_title }}</span></span>
      </a>
      {% endfor %}
    </div>
    <ol class="mt-8 flex flex-wrap items-center justify-center gap-x-4 gap-y-3 text-sm font-bold text-white/80" aria-label="Från prognos till uppföljning">
      {% assign stages = 'Prognos,Optimering,Budgivning,Drift,Uppföljning' | split: ',' %}
      {% for stage in stages %}<li class="flex items-center gap-4">{% unless forloop.first %}<span class="text-spring" aria-hidden="true">→</span>{% endunless %}{{ stage }}</li>{% endfor %}
    </ol>
  </section>

  <section id="zizzla-tjanster" class="scroll-mt-24 border-t border-white/10 py-16 lg:py-24" aria-labelledby="offer-title" data-service-explorer>
    <div class="mb-8 max-w-2xl">
      <p class="text-xs font-bold uppercase tracking-[0.2em] text-spring">Sex delar. En helhet.</p>
      <h2 id="offer-title" class="mt-4 text-3xl font-bold tracking-tight sm:text-4xl">Utforska ert nästa steg</h2>
      <p class="mt-4 leading-7 text-white/70">Välj en del av arbetsflödet och se hur den hänger ihop med resten.</p>
    </div>
    <div class="service-choices scroll-mt-24 grid grid-cols-2 gap-x-3 gap-y-4 sm:grid-cols-3 lg:grid-cols-6" aria-label="Välj tjänst" data-service-choices>
      {% for service in site.data.services %}
      <a id="service-tab-{{ service.id }}" href="#service-{{ service.id }}" data-service-choice="{{ service.id }}" class="service-choice group flex min-w-0 flex-col items-center gap-3 border-b-2 border-transparent px-1 py-4 text-center focus-visible:outline-2 focus-visible:outline-spring aria-selected:border-spring aria-selected:text-spring">
        <span class="service-symbol relative block h-20 w-20 overflow-hidden lg:h-28 lg:w-28">
          <img src="{{ '/assets/img/services/' | append: service.icon | relative_url }}" alt="" width="80" height="80" class="h-full w-full object-contain opacity-70 group-hover:opacity-100 group-aria-selected:opacity-100 {% if service.id == 'administration' or service.id == 'optimering' %}service-symbol--{{ service.id }}{% endif %}" loading="lazy">
        </span>
        <span class="flex items-center gap-2 text-xs font-bold leading-5 sm:text-sm"><span class="text-spring/70" aria-hidden="true">0{{ forloop.index }}</span>{{ service.short_title }}</span>
      </a>
      {% endfor %}
    </div>
    {% for service in site.data.services %}
    <section id="service-{{ service.id }}" data-service-content="{{ service.id }}" aria-labelledby="service-heading-{{ service.id }}" class="mt-6 scroll-mt-24 rounded-3xl bg-white p-5 text-navy sm:p-8 lg:p-10">
      <div class="grid min-w-0 gap-8 lg:grid-cols-5 lg:items-start lg:gap-10">
        <div class="min-w-0 lg:col-span-2">
          <p class="text-xs font-bold uppercase tracking-[0.15em] text-navy/50">{{ forloop.index | prepend: '0' }} / Zizzlas tjänster</p>
          <h3 id="service-heading-{{ service.id }}" class="mt-4 break-words text-2xl font-bold tracking-tight sm:text-3xl">{{ service.title }}</h3>
          <p class="mt-4 text-lg font-semibold leading-7">{{ service.value }}</p>
          <p class="mt-4 text-sm leading-7 text-navy/70">{{ service.text }}</p>
          <ul class="mt-6 space-y-3 text-sm font-medium">
            {% for benefit in service.benefits %}<li class="flex items-start gap-3"><span class="mt-1.5 size-2 shrink-0 rounded-full bg-spring" aria-hidden="true"></span>{{ benefit }}</li>{% endfor %}
          </ul>
        </div>
        <div class="min-w-0 lg:col-span-3">{% include service-visual.html service=service %}</div>
      </div>
    </section>
    {% endfor %}
  </section>

  <section class="border-t border-white/10 py-10 lg:py-12" aria-labelledby="day-title">
    <h2 id="day-title" class="text-3xl font-bold tracking-tight sm:text-4xl">Ett arbetsflöde genom hela dygnet</h2>
    <ol class="mt-6 grid gap-4 sm:grid-cols-2 lg:grid-cols-5">
      {% assign titles = 'Förstå morgondagen|Hitta bästa planen|Lägg bud|Kör säkert|Följ upp' | split: '|' %}
      {% assign descriptions = 'Pris- och lastprognoser.|Optimera resurser och marknader.|Granska och skicka realistiska bud.|Omsätt aktivering till kontrollerad drift.|Samla resultat, positioner och värde.' | split: '|' %}
      {% for title in titles %}
      <li class="grid grid-cols-[auto_1fr] gap-x-3 border-t border-spring/40 pt-3 lg:block"><span class="row-span-2 text-sm font-bold text-spring">0{{ forloop.index }}</span><h3 class="text-base font-bold lg:mt-2">{{ title }}</h3><p class="col-start-2 mt-1 text-sm leading-6 text-white/60">{{ descriptions[forloop.index0] }}</p></li>
      {% endfor %}
    </ol>
  </section>

  <section class="mb-16 rounded-3xl border border-spring/20 bg-white/5 px-6 py-12 text-center sm:px-12 sm:py-16">
    <h2 class="mx-auto max-w-2xl text-3xl font-bold tracking-tight sm:text-4xl">Nyfiken på hur Zizzla skulle fungera i er anläggning?</h2>
    <a href="mailto:{{ site.email }}" data-contact-open aria-haspopup="dialog" aria-controls="contact-dialog" class="mt-8 inline-flex rounded-full bg-spring px-8 py-4 font-bold text-navy hover:opacity-90 focus-visible:outline-2 focus-visible:outline-offset-4 focus-visible:outline-spring">Nyfiken? Hör av dig.</a>
  </section>
</div>

<script>
(() => {
  const explorer = document.querySelector('[data-service-explorer]');
  const choices = [...explorer.querySelectorAll('[data-service-choice]')];
  const panels = [...explorer.querySelectorAll('[data-service-content]')];
  const systemLinks = [...document.querySelectorAll('[data-system-service]')];
  const reducedMotion = window.matchMedia('(prefers-reduced-motion: reduce)');
  const select = (choice) => {
    choices.forEach(item => {
      item.setAttribute('aria-selected', String(item === choice));
      item.tabIndex = item === choice ? 0 : -1;
    });
    systemLinks.forEach(link => {
      if (link.dataset.systemService === choice.dataset.serviceChoice) link.setAttribute('aria-current', 'true');
      else link.removeAttribute('aria-current');
    });
    panels.forEach(panel => {
      panel.hidden = panel.dataset.serviceContent !== choice.dataset.serviceChoice;
      const video = panel.querySelector('video');
      if (video) {
        if (panel.hidden) video.pause();
        else if (!reducedMotion.matches) video.play().catch(() => {});
      }
    });
  };
  systemLinks.forEach(link => {
    link.addEventListener('click', event => {
      const choice = choices.find(item => item.dataset.serviceChoice === link.dataset.systemService);
      if (!choice) return;
      event.preventDefault();
      select(choice);
      explorer.querySelector('[data-service-choices]').scrollIntoView({ block: 'start', behavior: 'instant' });
      choice.focus({ preventScroll: true });
    });
  });
  explorer.querySelector('[data-service-choices]').setAttribute('role', 'tablist');
  choices.forEach((choice, index) => {
    choice.setAttribute('role', 'tab');
    choice.setAttribute('aria-controls', 'service-' + choice.dataset.serviceChoice);
    choice.addEventListener('click', event => {
      event.preventDefault();
      select(choice);
    });
    choice.addEventListener('keydown', event => {
      let next;
      if (event.key === 'ArrowRight') next = (index + 1) % choices.length;
      if (event.key === 'ArrowLeft') next = (index - 1 + choices.length) % choices.length;
      if (event.key === 'Home') next = 0;
      if (event.key === 'End') next = choices.length - 1;
      if (event.key === ' ') next = index;
      if (next === undefined) return;
      event.preventDefault();
      select(choices[next]);
      choices[next].focus({ preventScroll: true });
    });
  });
  panels.forEach(panel => {
    panel.setAttribute('role', 'tabpanel');
    panel.setAttribute('aria-labelledby', 'service-tab-' + panel.dataset.serviceContent);
    panel.tabIndex = 0;
  });
  select(choices.find(choice => choice.hash === window.location.hash) || choices[0]);
})();
</script>
