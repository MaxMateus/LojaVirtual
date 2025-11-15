<template>
  <MainLayout>
    <HeroBanner />

    <section class="space-y-6">
      <div class="flex flex-col gap-3 sm:flex-row sm:items-end sm:justify-between">
        <div>
          <p class="text-sm font-semibold uppercase tracking-widest text-slate-500">Seleção premium</p>
          <h2 class="text-3xl font-bold text-midnight">Produtos em destaque</h2>
          <p class="text-slate-500">Os favoritos da semana com frete grátis e cashback garantido.</p>
        </div>
        <div class="flex flex-wrap gap-2 text-sm font-medium text-slate-600">
          <button class="rounded-full border border-slate-200 px-4 py-2 transition hover:border-primary hover:text-primary">Todos</button>
          <button class="rounded-full border border-slate-200 px-4 py-2 transition hover:border-primary hover:text-primary">Smartphones</button>
          <button class="rounded-full border border-slate-200 px-4 py-2 transition hover:border-primary hover:text-primary">Periféricos</button>
          <button class="rounded-full border border-slate-200 px-4 py-2 transition hover:border-primary hover:text-primary">Games</button>
        </div>
      </div>

      <div class="grid gap-6 sm:grid-cols-2 xl:grid-cols-3">
        <ProductCard v-for="product in featuredProducts" :key="product.id" :product="product" />
      </div>
    </section>
  </MainLayout>
</template>

<script setup>
import HeroBanner from '../components/layout/HeroBanner.vue'
import MainLayout from '../components/layout/MainLayout.vue'
import ProductCard from '../components/ui/ProductCard.vue'

const featuredProducts = [
  {
    id: 1,
    title: 'Smartphone Orion X 256GB',
    description: 'Tela AMOLED 120Hz, câmera tripla 50MP e processador ultrarrápido para multitarefas.',
    price: '3.499,00',
    installment: '12x de R$ 291,58 s/ juros',
    image: 'https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?auto=format&fit=crop&w=800&q=80',
    badge: 'Lançamento',
    rating: '4,9',
    reviews: '3.2k',
    category: 'smartphones',
  },
  {
    id: 2,
    title: 'Notebook X-Performance 15"',
    description: 'Intel Core i9, 32GB RAM e SSD NVMe 1TB para produtividade máxima.',
    price: '8.199,00',
    installment: '10x de R$ 819,90 s/ juros',
    image: 'https://images.unsplash.com/photo-1517336714731-489689fd1ca8?auto=format&fit=crop&w=900&q=80',
    badge: 'Frete grátis',
    rating: '4,8',
    reviews: '1.1k',
    category: 'notebooks',
  },
  {
    id: 3,
    title: 'Headset Pro Sound 7.1',
    description: 'Conforto extremo, cancelamento ativo de ruído e drivers de alta fidelidade.',
    price: '899,90',
    installment: '8x de R$ 112,48 s/ juros',
    image: 'https://images.unsplash.com/photo-1484704849700-f032a568e944?auto=format&fit=crop&w=900&q=80',
    badge: 'Mais vendido',
    rating: '4,7',
    reviews: '5.8k',
    category: 'periféricos',
  },
  {
    id: 4,
    title: 'Monitor UltraWide 34"',
    description: 'Painel QHD, 144Hz, HDR600 e ajuste ergonômico completo para criar e jogar.',
    price: '3.899,00',
    installment: '12x de R$ 324,91 s/ juros',
    image: 'https://images.unsplash.com/photo-1461749280684-dccba630e2f6?auto=format&fit=crop&w=900&q=80',
    badge: 'Cashback',
    rating: '4,9',
    reviews: '2.4k',
    category: 'monitores',
  },
  {
    id: 5,
    title: 'Mouse Gamer Carbon',
    description: 'Sensor 26k DPI, iluminação RGB inteligente e até 180h de bateria.',
    price: '499,90',
    installment: '6x de R$ 83,31 s/ juros',
    image: 'https://images.unsplash.com/photo-1587202372775-98973d29d453?auto=format&fit=crop&w=900&q=80',
    badge: 'Promoção',
    rating: '4,6',
    reviews: '9.4k',
    category: 'acessórios',
  },
  {
    id: 6,
    title: 'Console Next-Gen 1TB',
    description: 'Experiência 4K com 120fps, ray tracing e catálogo exclusivo de jogos.',
    price: '4.299,00',
    installment: '10x de R$ 429,90 s/ juros',
    image: 'https://images.unsplash.com/photo-1605901309584-818e25960a8f?auto=format&fit=crop&w=900&q=80',
    badge: 'Novo',
    rating: '4,9',
    reviews: '7.1k',
    category: 'games',
  },
]
</script>
