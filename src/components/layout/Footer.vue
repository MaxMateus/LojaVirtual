<template>
  <footer class="border-t border-slate-200 bg-white">
    <div class="mx-auto max-w-7xl px-4 py-10 text-center text-sm text-slate-500 sm:px-6 lg:px-8">
      <div class="flex flex-col items-center gap-3">
        <p class="text-base font-semibold text-midnight">LojaVirtual</p>
        <p>Experiência premium em tecnologia com frete rápido e suporte especializado.</p>
        <div class="flex flex-wrap justify-center gap-6 text-xs uppercase tracking-wide text-slate-400">
          <span>Política de privacidade</span>
          <span>Termos de uso</span>
          <span>Atendimento</span>
          <span>Trabalhe conosco</span>
        </div>
      </div>
      <p class="mt-6 text-xs text-slate-400">© {{ new Date().getFullYear() }} LojaVirtual. Todos os direitos reservados.</p>
    </div>
  </footer>
</template>
