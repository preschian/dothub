<template>
  <div class="min-h-screen bg-gradient-to-br from-slate-50/50 via-white to-primary-50/20">
    <!-- Navigation -->
    <nav class="relative">
      <!-- Background with blur effect -->
      <div class="absolute inset-0 bg-white/80 backdrop-blur-md border-b border-white/50" />

      <!-- Navigation content -->
      <div class="relative py-4">
        <UContainer>
          <div class="flex items-center justify-between">
            <!-- Logo Section -->
            <div class="flex items-center gap-3">
              <div class="w-10 h-10 bg-gradient-to-br from-primary-500 to-primary-600 rounded-xl flex items-center justify-center shadow-lg shadow-primary-500/25">
                <Icon name="i-lucide-link" class="w-5 h-5 text-white" />
              </div>
              <div>
                <span class="text-xl font-bold bg-gradient-to-r from-slate-900 to-slate-600 bg-clip-text text-transparent">DotMe</span>
                <div class="text-xs text-slate-500 -mt-1">
                  Decentralized Links
                </div>
              </div>
            </div>

            <!-- Navigation Actions -->
            <div class="flex items-center gap-3">
              <UButton
                variant="ghost"
                size="sm"
                class="text-slate-600 hover:text-slate-900 hover:bg-slate-100/50"
                icon="i-lucide-compass"
              >
                Discover
              </UButton>

              <div class="hidden sm:block w-px h-6 bg-slate-200" />

              <UButton
                variant="outline"
                size="sm"
                class="border-slate-200 hover:border-primary-300 hover:bg-primary-50"
                icon="i-lucide-user"
              >
                Sign In
              </UButton>

              <UButton
                size="sm"
                class="bg-gradient-to-r from-primary-500 to-primary-600 hover:from-primary-600 hover:to-primary-700 shadow-lg shadow-primary-500/25"
                icon="i-lucide-plus"
              >
                Get Started
              </UButton>
            </div>
          </div>
        </UContainer>
      </div>
    </nav>

    <!-- Page Content -->
    <slot />

    <!-- Footer -->
    <footer class="bg-gradient-to-r from-slate-50 to-white border-t border-slate-200/50">
      <UContainer>
        <div class="py-12">
          <div class="flex flex-col md:flex-row justify-between items-center">
            <!-- Footer Logo -->
            <div class="flex items-center gap-3 mb-6 md:mb-0">
              <div class="w-8 h-8 bg-gradient-to-br from-primary-500 to-primary-600 rounded-lg flex items-center justify-center">
                <Icon name="i-lucide-link" class="w-4 h-4 text-white" />
              </div>
              <div>
                <span class="text-lg font-semibold text-slate-900">DotMe</span>
                <div class="text-xs text-slate-500 -mt-1">
                  Decentralized Links
                </div>
              </div>
            </div>

            <!-- Footer Links -->
            <div class="flex flex-col sm:flex-row items-center gap-6 text-sm">
              <div class="flex items-center gap-6 text-slate-600">
                <a href="#" class="hover:text-primary-600 transition-colors flex items-center gap-2">
                  <Icon name="i-lucide-shield-check" class="w-4 h-4" />
                  Privacy
                </a>
                <a href="#" class="hover:text-primary-600 transition-colors flex items-center gap-2">
                  <Icon name="i-lucide-file-text" class="w-4 h-4" />
                  Terms
                </a>
                <a href="#" class="hover:text-primary-600 transition-colors flex items-center gap-2">
                  <Icon name="i-lucide-help-circle" class="w-4 h-4" />
                  Support
                </a>
              </div>
              <div class="text-slate-500">
                © {{ new Date().getFullYear() }} DotMe. Built on Polkadot.
              </div>
            </div>
          </div>

          <!-- Additional Footer Info -->
          <div class="mt-8 pt-8 border-t border-slate-200/50">
            <div class="flex flex-col sm:flex-row justify-between items-center gap-4 text-xs text-slate-500">
              <div class="flex items-center gap-4">
                <div class="flex items-center gap-2">
                  <div class="w-2 h-2 bg-green-500 rounded-full" />
                  <span>All systems operational</span>
                </div>
                <div class="flex items-center gap-2">
                  <Icon name="i-lucide-globe" class="w-3 h-3" />
                  <span>Deployed on IPFS</span>
                </div>
              </div>
              <div class="flex items-center gap-4">
                <a href="#" class="hover:text-slate-700 transition-colors">
                  <Icon name="i-lucide-twitter" class="w-4 h-4" />
                </a>
                <a href="#" class="hover:text-slate-700 transition-colors">
                  <Icon name="i-lucide-github" class="w-4 h-4" />
                </a>
                <a href="#" class="hover:text-slate-700 transition-colors">
                  <Icon name="i-lucide-message-circle" class="w-4 h-4" />
                </a>
              </div>
            </div>
          </div>
        </div>
      </UContainer>
    </footer>
  </div>
</template>
