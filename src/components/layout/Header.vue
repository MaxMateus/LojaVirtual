<template>
  <header class="sticky top-0 z-50 border-b border-slate-100 bg-white/90 backdrop-blur">
    <div class="max-w-7xl mx-auto flex flex-col gap-4 px-4 py-4 sm:px-6 lg:flex-row lg:items-center lg:gap-8 lg:px-8">
      <div class="flex items-center gap-3">
        <div class="flex h-11 w-11 items-center justify-center rounded-2xl bg-primary/10 text-lg font-semibold text-primary">
          LV
        </div>
        <div>
          <p class="text-lg font-bold text-midnight">LojaVirtual</p>
          <p class="hidden text-xs font-medium text-slate-500 sm:block">Tecnologia e inovação ao seu alcance</p>
        </div>
      </div>

      <div class="w-full lg:flex-1">
        <label class="relative flex items-center">
          <span class="pointer-events-none absolute inset-y-0 left-4 flex items-center text-slate-400">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.8">
              <path stroke-linecap="round" stroke-linejoin="round" d="m21 21-4.35-4.35M11 19a8 8 0 1 0 0-16 8 8 0 0 0 0 16z" />
            </svg>
          </span>
          <input
            type="search"
            placeholder="Buscar por produtos, marcas ou categorias"
            class="w-full rounded-full border border-slate-200 bg-slate-50 py-2.5 pl-12 pr-28 text-sm text-slate-700 transition focus:border-primary focus:bg-white focus:outline-none focus:ring-2 focus:ring-primary/20"
          />
          <span class="absolute right-1 inline-flex items-center">
            <button class="rounded-full bg-primary px-4 py-2 text-sm font-semibold text-white transition hover:bg-primary-dark">
              Buscar
            </button>
          </span>
        </label>
      </div>

      <nav class="flex flex-wrap items-center gap-3 text-sm font-medium text-slate-600">
        <router-link to="/" class="rounded-full px-3 py-1.5 transition hover:bg-slate-100 hover:text-primary">
          Lançamentos
        </router-link>
        <router-link to="/ofertas" class="rounded-full px-3 py-1.5 transition hover:bg-slate-100 hover:text-primary">
          Ofertas do dia
        </router-link>
        <router-link to="/suporte" class="rounded-full px-3 py-1.5 transition hover:bg-slate-100 hover:text-primary">
          Suporte
        </router-link>
        <div class="flex items-center gap-2">
          <router-link
            to="/login"
            class="inline-flex items-center gap-1 rounded-full border border-slate-200 px-4 py-2 text-slate-700 transition hover:border-primary hover:text-primary"
          >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.8">
              <path stroke-linecap="round" stroke-linejoin="round" d="M15 7a3 3 0 1 1-6 0 3 3 0 0 1 6 0ZM5 21a7 7 0 0 1 14 0" />
            </svg>
            Entrar
          </router-link>
          <router-link
            to="/cart"
            class="inline-flex items-center gap-2 rounded-full bg-primary/10 px-4 py-2 text-primary transition hover:bg-primary/20"
          >
            <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="1.8">
              <path stroke-linecap="round" stroke-linejoin="round" d="M2.5 4.5h2.153a1 1 0 0 1 .981.804l1.63 8.147A1 1 0 0 0 8.24 14.5h8.764a1 1 0 0 0 .978-.804l1.266-6.174a1 1 0 0 0-.978-1.196H6.5" />
              <path stroke-linecap="round" stroke-linejoin="round" d="M9 20.5a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0zm9 0a.75.75 0 1 1-1.5 0 .75.75 0 0 1 1.5 0z" />
            </svg>
            Carrinho
          </router-link>
        </div>
      </nav>
    </div>
  </header>
</template>
