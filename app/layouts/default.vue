<template>
  <div class="min-h-screen">
    <!-- Navigation -->
    <nav class="py-8">
      <UContainer>
        <div class="flex items-center justify-between">
          <div class="flex items-center gap-3">
            <div class="w-8 h-8 bg-primary-600 rounded-lg" />
            <span class="text-xl font-semibold text-slate-900">DotMe</span>
          </div>
          <div class="flex items-center gap-4">
            <UButton variant="outline" size="sm">
              Discover
            </UButton>
            <UButton variant="ghost" size="sm">
              Sign In
            </UButton>
          </div>
        </div>
      </UContainer>
    </nav>

    <!-- Page Content -->
    <slot />

    <!-- Footer -->
    <footer class="bg-white border-t border-slate-200 py-12">
      <UContainer>
        <div class="flex flex-col md:flex-row justify-between items-center">
          <div class="flex items-center gap-3 mb-4 md:mb-0">
            <div class="w-8 h-8 bg-primary-600 rounded-lg" />
            <span class="text-xl font-semibold text-slate-900">DotMe</span>
          </div>
          <div class="flex items-center gap-6 text-sm text-slate-600">
            <a href="#" class="hover:text-slate-900 transition-colors">Privacy</a>
            <a href="#" class="hover:text-slate-900 transition-colors">Terms</a>
            <a href="#" class="hover:text-slate-900 transition-colors">Support</a>
            <span>© {{ new Date().getFullYear() }} DotMe</span>
          </div>
        </div>
      </UContainer>
    </footer>
  </div>
</template>
