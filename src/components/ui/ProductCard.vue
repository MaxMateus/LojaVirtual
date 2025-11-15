<script setup>
const props = defineProps({
  product: {
    type: Object,
    required: true,
  },
})
</script>

<template>
  <article class="group relative flex h-full flex-col rounded-3xl bg-white p-5 shadow-soft transition duration-300 hover:-translate-y-1 hover:shadow-elevated">
    <div class="relative overflow-hidden rounded-2xl bg-slate-100">
      <img :src="props.product.image" :alt="props.product.title" class="h-52 w-full object-cover transition duration-500 group-hover:scale-105" />
      <span
        v-if="props.product.badge"
        class="absolute left-4 top-4 rounded-full bg-accent px-3 py-1 text-xs font-semibold uppercase tracking-wide text-slate-900"
      >
        {{ props.product.badge }}
      </span>
    </div>

    <div class="mt-5 flex flex-1 flex-col">
      <p class="text-xs uppercase tracking-[0.2em] text-slate-400">{{ props.product.category }}</p>
      <h3 class="mt-1 text-lg font-semibold text-midnight">{{ props.product.title }}</h3>
      <p class="mt-2 text-sm text-slate-500">{{ props.product.description }}</p>

      <div class="mt-4 flex items-center gap-3 text-sm text-slate-500">
        <div class="flex items-center gap-1 text-amber-400">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" viewBox="0 0 24 24" fill="currentColor">
            <path
              d="M12 .587l3.668 7.425 8.2 1.193-5.934 5.636 1.402 8.159L12 18.896l-7.336 3.104 1.402-8.159L.132 9.205l8.2-1.193z"
            />
          </svg>
          <span class="font-semibold text-slate-700">{{ props.product.rating }}</span>
        </div>
        <span>({{ props.product.reviews }} avaliações)</span>
      </div>

      <div class="mt-5">
        <p class="text-sm text-slate-500">a partir de</p>
        <p class="text-2xl font-bold text-midnight">R$ {{ props.product.price }}</p>
        <p class="text-xs text-success">{{ props.product.installment }}</p>
      </div>

      <div class="mt-auto pt-4">
        <button
          class="flex w-full items-center justify-center gap-2 rounded-2xl bg-primary py-3 text-sm font-semibold text-white transition hover:bg-primary-dark"
        >
          Adicionar ao carrinho
        </button>
      </div>
    </div>
  </article>
</template>
