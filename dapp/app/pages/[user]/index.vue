<script setup lang="ts">
definePageMeta({
  layout: 'empty',
})
</script>

<template>
  <div class="min-h-screen bg-gradient-to-br from-slate-100 via-white to-primary-100/30">
    <UContainer>
      <!-- Profile Header -->
      <div class="pt-12 pb-8">
        <div class="max-w-2xl mx-auto text-center relative">
          <!-- Burger Menu - Top Right -->
          <div class="absolute top-0 right-0 z-10">
            <UModal>
              <UButton
                icon="i-lucide-more-horizontal"
                size="sm"
                color="neutral"
                variant="ghost"
                class="rounded-full"
              />

              <template #header>
                <h3 class="text-lg font-semibold">
                  Page Actions
                </h3>
              </template>

              <template #body>
                <div class="space-y-3">
                  <UButton
                    variant="ghost"
                    class="w-full justify-start gap-3 p-4 h-auto"
                    size="lg"
                    @click="() => {}"
                  >
                    <div class="w-10 h-10 bg-blue-100 rounded-full flex items-center justify-center">
                      <Icon name="i-lucide-share-2" class="w-5 h-5 text-blue-600" />
                    </div>
                    <div class="text-left">
                      <div class="font-medium">
                        Share Page
                      </div>
                      <div class="text-sm text-slate-500">
                        Share this profile with others
                      </div>
                    </div>
                  </UButton>

                  <UButton
                    variant="ghost"
                    class="w-full justify-start gap-3 p-4 h-auto"
                    size="lg"
                    @click="() => {}"
                  >
                    <div class="w-10 h-10 bg-green-100 rounded-full flex items-center justify-center">
                      <Icon name="i-lucide-bookmark" class="w-5 h-5 text-green-600" />
                    </div>
                    <div class="text-left">
                      <div class="font-medium">
                        Save
                      </div>
                      <div class="text-sm text-slate-500">
                        Save this profile to your favorites
                      </div>
                    </div>
                  </UButton>

                  <UButton
                    variant="ghost"
                    class="w-full justify-start gap-3 p-4 h-auto"
                    size="lg"
                    @click="() => {}"
                  >
                    <div class="w-10 h-10 bg-red-100 rounded-full flex items-center justify-center">
                      <Icon name="i-lucide-flag" class="w-5 h-5 text-red-600" />
                    </div>
                    <div class="text-left">
                      <div class="font-medium">
                        Report
                      </div>
                      <div class="text-sm text-slate-500">
                        Report inappropriate content
                      </div>
                    </div>
                  </UButton>
                </div>
              </template>
            </UModal>
          </div>

          <!-- Profile Avatar -->
          <div class="relative mb-6 flex justify-center">
            <div class="relative">
              <div class="w-24 h-24 bg-gradient-to-br from-primary-500 to-primary-600 rounded-full flex items-center justify-center ring-4 ring-white shadow-xl">
                <Icon name="i-lucide-user" class="w-12 h-12 text-white" />
              </div>
              <!-- Verification Badge -->
              <div class="absolute -bottom-1 -right-1 w-8 h-8 bg-gradient-to-br from-green-500 to-green-600 rounded-full flex items-center justify-center ring-4 ring-white shadow-lg">
                <Icon name="i-lucide-check" class="w-4 h-4 text-white" />
              </div>
            </div>
          </div>

          <!-- User Info -->
          <h1 class="text-3xl font-bold text-slate-900 mb-2">
            @{{ $route.params.user }}
          </h1>
          <p class="text-slate-600 mb-6">
            Building the future on Polkadot blockchain ⚡ Creative developer & NFT enthusiast
          </p>

          <!-- Wallet Address -->
          <div class="flex items-center justify-center gap-3">
            <div class="inline-flex items-center gap-2 bg-white/80 backdrop-blur-sm border border-white/50 rounded-full px-4 py-2 text-sm text-slate-600">
              <Icon name="i-lucide-wallet" class="w-4 h-4 text-primary-600" />
              <span class="font-mono">5GrwvaEF...KutQY</span>
              <button class="hover:text-primary-600 transition-colors">
                <Icon name="i-lucide-copy" class="w-4 h-4" />
              </button>
            </div>

            <!-- Send DOT Modal -->
            <UModal>
              <UButton
                size="sm"
                icon="i-lucide-send"
                class="bg-primary-600 hover:bg-primary-700"
              >
                Send DOT
              </UButton>

              <template #header>
                <div class="flex items-center gap-3">
                  <div class="w-10 h-10 bg-primary-100 rounded-full flex items-center justify-center">
                    <Icon name="i-lucide-heart" class="w-5 h-5 text-primary-600" />
                  </div>
                  <div>
                    <h3 class="text-lg font-semibold">
                      Support @{{ $route.params.user }}
                    </h3>
                    <p class="text-sm text-slate-500">
                      Send cryptocurrency to show your appreciation
                    </p>
                  </div>
                </div>
              </template>

              <template #body>
                <div class="space-y-6">
                  <!-- Wallet Address Display -->
                  <div class="bg-slate-50 rounded-xl p-4">
                    <label class="text-sm font-medium text-slate-700 mb-2 block">Wallet Address</label>
                    <div class="flex items-center gap-2 bg-white rounded-lg p-3 border border-slate-200">
                      <Icon name="i-lucide-wallet" class="w-4 h-4 text-slate-400" />
                      <span class="font-mono text-sm flex-1">5GrwvaEF5j4wN9qN9M2KutQY</span>
                      <button class="text-slate-400 hover:text-slate-600 transition-colors">
                        <Icon name="i-lucide-copy" class="w-4 h-4" />
                      </button>
                    </div>
                  </div>

                  <!-- Quick Amount Buttons -->
                  <div>
                    <label class="text-sm font-medium text-slate-700 mb-3 block">Quick Amounts</label>
                    <div class="grid grid-cols-3 gap-3">
                      <UButton variant="outline" class="justify-center" size="sm">
                        <Icon name="i-lucide-coffee" class="w-4 h-4 mr-2" />
                        1 DOT
                      </UButton>
                      <UButton variant="outline" class="justify-center" size="sm">
                        <Icon name="i-lucide-heart" class="w-4 h-4 mr-2" />
                        5 DOT
                      </UButton>
                      <UButton variant="outline" class="justify-center" size="sm">
                        <Icon name="i-lucide-star" class="w-4 h-4 mr-2" />
                        10 DOT
                      </UButton>
                    </div>
                  </div>

                  <!-- Message -->
                  <div>
                    <label class="text-sm font-medium text-slate-700 mb-2 block">Message (Optional)</label>
                    <textarea
                      class="w-full p-3 border border-slate-200 rounded-lg text-sm resize-none"
                      rows="3"
                      placeholder="Say something nice..."
                    />
                  </div>
                </div>
              </template>

              <template #footer>
                <div class="flex gap-3 w-full">
                  <UButton variant="outline" class="flex-1">
                    Cancel
                  </UButton>
                  <UButton class="flex-1">
                    <Icon name="i-lucide-send" class="w-4 h-4 mr-2" />
                    Send DOT
                  </UButton>
                </div>
              </template>
            </UModal>
          </div>
        </div>
      </div>

      <!-- Main Content -->
      <div class="max-w-2xl mx-auto pb-12">
        <!-- Links Section -->
        <div class="space-y-3 mb-12">
          <!-- Social Link -->
          <a href="#" class="flex items-center justify-between p-4 bg-white/90 hover:bg-white rounded-xl border border-slate-200/50 hover:border-blue-300 group transition-all duration-200 hover:shadow-md">
            <div class="flex items-center gap-3">
              <div class="w-10 h-10 bg-blue-500 rounded-lg flex items-center justify-center">
                <Icon name="i-lucide-twitter" class="w-5 h-5 text-white" />
              </div>
              <div>
                <h3 class="font-medium text-slate-900 group-hover:text-blue-600 transition-colors">Follow me on Twitter</h3>
                <p class="text-sm text-slate-500">@{{ $route.params.user }}</p>
              </div>
            </div>
            <Icon name="i-lucide-external-link" class="w-4 h-4 text-slate-400 group-hover:text-blue-500 transition-colors" />
          </a>

          <!-- GitHub Link -->
          <a href="#" class="flex items-center justify-between p-4 bg-white/90 hover:bg-white rounded-xl border border-slate-200/50 hover:border-gray-300 group transition-all duration-200 hover:shadow-md">
            <div class="flex items-center gap-3">
              <div class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center">
                <Icon name="i-lucide-github" class="w-5 h-5 text-white" />
              </div>
              <div>
                <h3 class="font-medium text-slate-900 group-hover:text-gray-700 transition-colors">Check out my code</h3>
                <p class="text-sm text-slate-500">github.com/{{ $route.params.user }}</p>
              </div>
            </div>
            <Icon name="i-lucide-external-link" class="w-4 h-4 text-slate-400 group-hover:text-gray-700 transition-colors" />
          </a>

          <!-- Website Link -->
          <a href="#" class="flex items-center justify-between p-4 bg-white/90 hover:bg-white rounded-xl border border-slate-200/50 hover:border-green-300 group transition-all duration-200 hover:shadow-md">
            <div class="flex items-center gap-3">
              <div class="w-10 h-10 bg-green-500 rounded-lg flex items-center justify-center">
                <Icon name="i-lucide-globe" class="w-5 h-5 text-white" />
              </div>
              <div>
                <h3 class="font-medium text-slate-900 group-hover:text-green-600 transition-colors">Visit my website</h3>
                <p class="text-sm text-slate-500">www.{{ $route.params.user }}.com</p>
              </div>
            </div>
            <Icon name="i-lucide-external-link" class="w-4 h-4 text-slate-400 group-hover:text-green-500 transition-colors" />
          </a>

          <!-- Portfolio Link -->
          <a href="#" class="flex items-center justify-between p-4 bg-white/90 hover:bg-white rounded-xl border border-slate-200/50 hover:border-purple-300 group transition-all duration-200 hover:shadow-md">
            <div class="flex items-center gap-3">
              <div class="w-10 h-10 bg-purple-500 rounded-lg flex items-center justify-center">
                <Icon name="i-lucide-briefcase" class="w-5 h-5 text-white" />
              </div>
              <div>
                <h3 class="font-medium text-slate-900 group-hover:text-purple-600 transition-colors">View my portfolio</h3>
                <p class="text-sm text-slate-500">My latest projects and work</p>
              </div>
            </div>
            <Icon name="i-lucide-external-link" class="w-4 h-4 text-slate-400 group-hover:text-purple-500 transition-colors" />
          </a>
        </div>

        <!-- NFT Collection Section -->
        <div class="mb-12">
          <div class="flex items-center justify-between mb-6">
            <h2 class="text-xl font-semibold text-slate-900">
              NFT Collection
            </h2>
            <a href="#" class="text-sm text-primary-600 hover:text-primary-700 transition-colors">
              View all
            </a>
          </div>

          <div class="space-y-6">
            <!-- Featured NFT (larger) -->
            <div class="group cursor-pointer">
              <div class="bg-gradient-to-br from-slate-900 to-slate-800 rounded-2xl p-6 text-white hover:shadow-2xl transition-all duration-300">
                <div class="flex items-center gap-4 mb-4">
                  <div class="w-16 h-16 bg-gradient-to-br from-primary-500 to-primary-600 rounded-xl flex items-center justify-center">
                    <Icon name="i-lucide-image" class="w-8 h-8 text-white" />
                  </div>
                  <div class="flex-1">
                    <h3 class="text-lg font-semibold mb-1">
                      Cool NFT #001
                    </h3>
                    <p class="text-slate-300 text-sm">
                      Featured Collection
                    </p>
                  </div>
                  <div class="text-right">
                    <p class="text-2xl font-bold">
                      0.5 DOT
                    </p>
                    <p class="text-slate-400 text-sm">
                      ~$2.50
                    </p>
                  </div>
                </div>
                <div class="flex items-center justify-between text-sm text-slate-400">
                  <span>Minted Dec 2024</span>
                  <span>1 of 1</span>
                </div>
              </div>
            </div>

            <!-- Regular NFTs - Row Layout -->
            <div class="space-y-3">
              <!-- Regular NFT 1 -->
              <div class="group cursor-pointer">
                <div class="bg-white rounded-xl p-4 border border-slate-200 hover:border-orange-300 hover:shadow-lg transition-all duration-200">
                  <div class="flex items-center gap-4">
                    <div class="w-16 h-16 bg-gradient-to-br from-orange-500 to-red-500 rounded-lg flex items-center justify-center flex-shrink-0">
                      <Icon name="i-lucide-palette" class="w-8 h-8 text-white" />
                    </div>
                    <div class="flex-1 min-w-0">
                      <h3 class="font-medium text-slate-900 mb-1">
                        Art Piece #042
                      </h3>
                      <p class="text-sm text-slate-600 hidden sm:block mb-2">
                        Beautiful digital artwork with vibrant colors and abstract patterns.
                      </p>
                      <div class="flex items-center gap-3">
                        <span class="text-lg font-semibold text-slate-900">1.2 DOT</span>
                        <span class="text-xs text-slate-500 bg-slate-100 px-2 py-1 rounded-full">Digital Art</span>
                      </div>
                    </div>
                    <div class="text-right flex-shrink-0">
                      <Icon name="i-lucide-external-link" class="w-5 h-5 text-slate-400 group-hover:text-orange-500 transition-colors" />
                    </div>
                  </div>
                </div>
              </div>

              <!-- Regular NFT 2 -->
              <div class="group cursor-pointer">
                <div class="bg-white rounded-xl p-4 border border-slate-200 hover:border-blue-300 hover:shadow-lg transition-all duration-200">
                  <div class="flex items-center gap-4">
                    <div class="w-16 h-16 bg-gradient-to-br from-blue-500 to-purple-600 rounded-lg flex items-center justify-center flex-shrink-0">
                      <Icon name="i-lucide-zap" class="w-8 h-8 text-white" />
                    </div>
                    <div class="flex-1 min-w-0">
                      <h3 class="font-medium text-slate-900 mb-1">
                        Digital Wave
                      </h3>
                      <p class="text-sm text-slate-600 hidden sm:block mb-2">
                        Dynamic wave patterns created with advanced generative algorithms.
                      </p>
                      <div class="flex items-center gap-3">
                        <span class="text-lg font-semibold text-slate-900">0.8 DOT</span>
                        <span class="text-xs text-slate-500 bg-slate-100 px-2 py-1 rounded-full">Abstract</span>
                      </div>
                    </div>
                    <div class="text-right flex-shrink-0">
                      <Icon name="i-lucide-external-link" class="w-5 h-5 text-slate-400 group-hover:text-blue-500 transition-colors" />
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Footer Info -->
        <div class="text-center mt-12 pt-8 border-t border-slate-200/50">
          <p class="text-sm text-slate-500 mb-4">
            Powered by DotMe - Decentralized links on Polkadot
          </p>
          <div class="flex items-center justify-center gap-2 text-xs text-slate-400">
            <div class="w-2 h-2 bg-green-500 rounded-full" />
            <span>Verified on blockchain</span>
          </div>
        </div>
      </div>
    </UContainer>
  </div>
</template>
