<template>
  <section class="relative overflow-hidden rounded-3xl bg-gradient-to-r from-primary to-primary-dark px-6 py-10 text-white shadow-elevated sm:px-12">
    <div class="space-y-6 sm:max-w-2xl">
      <p class="inline-flex items-center gap-2 rounded-full bg-white/15 px-4 py-1 text-sm font-medium uppercase tracking-wide text-white/90">
        <span class="h-2 w-2 rounded-full bg-accent"></span>
        ofertas exclusivas desta semana
      </p>
      <h1 class="text-3xl font-bold leading-tight sm:text-4xl">
        Tudo o que você precisa para montar o setup perfeito
      </h1>
      <p class="text-base text-white/85 sm:text-lg">
        Smartphones, notebooks, periféricos e muito mais com entrega rápida, cashback em dobro e parcelamento em até 12x sem juros.
      </p>
      <div class="flex flex-wrap items-center gap-4">
        <button class="rounded-full bg-white px-6 py-3 text-sm font-semibold text-primary transition hover:bg-slate-100">
          Ver lançamentos
        </button>
        <button class="rounded-full border border-white/40 px-6 py-3 text-sm font-semibold text-white transition hover:border-white hover:bg-white/10">
          Explorar categorias
        </button>
      </div>
      <div class="flex flex-wrap gap-6 text-sm text-white/80">
        <div>
          <p class="text-2xl font-bold text-white">+2M</p>
          <p>Clientes satisfeitos</p>
        </div>
        <div>
          <p class="text-2xl font-bold text-white">24h</p>
          <p>Envio para capitais</p>
        </div>
        <div>
          <p class="text-2xl font-bold text-white">12x</p>
          <p>Parcelamento sem juros</p>
        </div>
      </div>
    </div>

    <div class="pointer-events-none absolute -right-6 bottom-0 hidden translate-y-12 scale-110 sm:block">
      <div class="glass-surface rounded-[2.5rem] p-6 text-midnight">
        <p class="text-sm font-medium text-slate-500">Destaque do dia</p>
        <p class="mt-2 text-xl font-semibold text-midnight">Combo gamer com 20% off</p>
        <p class="text-sm text-slate-500">Apenas hoje</p>
      </div>
    </div>
  </section>
</template>
