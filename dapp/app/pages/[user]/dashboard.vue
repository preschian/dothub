<template>
  <div class="min-h-screen bg-gradient-to-br from-slate-200 via-white to-primary-200/30">
    <UContainer>
      <!-- Dashboard Header -->
      <div class="mb-8 pt-8">
        <div class="flex flex-col md:flex-row md:items-center justify-between gap-4">
          <div>
            <h1 class="text-3xl font-bold text-slate-900 mb-2">
              Dashboard
            </h1>
            <p class="text-slate-600">
              Manage your decentralized link page
            </p>
          </div>
          <div class="flex gap-3">
            <UButton variant="outline" size="sm" icon="i-lucide-eye">
              Preview Page
            </UButton>
            <UButton size="sm" icon="i-lucide-share-2">
              Share Page
            </UButton>
          </div>
        </div>
      </div>

      <!-- Stats Cards -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
        <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm hover:shadow-md transition-shadow">
          <div class="flex items-center justify-between mb-4">
            <h3 class="text-sm font-medium text-slate-600">
              Total Clicks
            </h3>
            <div class="w-10 h-10 bg-gradient-to-br from-primary-500 to-primary-600 rounded-lg flex items-center justify-center">
              <Icon name="i-lucide-mouse-pointer" class="w-5 h-5 text-white" />
            </div>
          </div>
          <div class="text-2xl font-bold text-slate-900 mb-1">
            1,234
          </div>
          <div class="text-sm text-primary-600 font-medium">
            +12% from last month
          </div>
        </div>

        <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm hover:shadow-md transition-shadow">
          <div class="flex items-center justify-between mb-4">
            <h3 class="text-sm font-medium text-slate-600">
              Page Views
            </h3>
            <div class="w-10 h-10 bg-gradient-to-br from-blue-500 to-blue-600 rounded-lg flex items-center justify-center">
              <Icon name="i-lucide-eye" class="w-5 h-5 text-white" />
            </div>
          </div>
          <div class="text-2xl font-bold text-slate-900 mb-1">
            892
          </div>
          <div class="text-sm text-blue-600 font-medium">
            +8% from last month
          </div>
        </div>

        <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm hover:shadow-md transition-shadow">
          <div class="flex items-center justify-between mb-4">
            <h3 class="text-sm font-medium text-slate-600">
              Active Links
            </h3>
            <div class="w-10 h-10 bg-gradient-to-br from-purple-500 to-purple-600 rounded-lg flex items-center justify-center">
              <Icon name="i-lucide-link" class="w-5 h-5 text-white" />
            </div>
          </div>
          <div class="text-2xl font-bold text-slate-900 mb-1">
            12
          </div>
          <div class="text-sm text-slate-600">
            5 published
          </div>
        </div>

        <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm hover:shadow-md transition-shadow">
          <div class="flex items-center justify-between mb-4">
            <h3 class="text-sm font-medium text-slate-600">
              NFTs Listed
            </h3>
            <div class="w-10 h-10 bg-gradient-to-br from-orange-500 to-orange-600 rounded-lg flex items-center justify-center">
              <Icon name="i-lucide-image" class="w-5 h-5 text-white" />
            </div>
          </div>
          <div class="text-2xl font-bold text-slate-900 mb-1">
            3
          </div>
          <div class="text-sm text-slate-600">
            2 collections
          </div>
        </div>
      </div>

      <div class="grid lg:grid-cols-3 gap-8 pb-8">
        <!-- Main Content -->
        <div class="lg:col-span-2 space-y-6">
          <!-- Quick Actions -->
          <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm">
            <h2 class="text-lg font-semibold text-slate-900 mb-4">
              Quick Actions
            </h2>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
              <button class="flex flex-col items-center p-4 rounded-xl border border-slate-200/50 hover:border-primary-300 hover:bg-gradient-to-br hover:from-primary-50 hover:to-primary-100/50 transition-all duration-200 group">
                <div class="w-12 h-12 bg-gradient-to-br from-primary-500 to-primary-600 rounded-xl flex items-center justify-center mb-3 group-hover:scale-110 transition-transform">
                  <Icon name="i-lucide-plus" class="w-6 h-6 text-white" />
                </div>
                <span class="text-sm font-medium text-slate-700">Add Link</span>
              </button>

              <button class="flex flex-col items-center p-4 rounded-xl border border-slate-200/50 hover:border-primary-300 hover:bg-gradient-to-br hover:from-primary-50 hover:to-primary-100/50 transition-all duration-200 group">
                <div class="w-12 h-12 bg-gradient-to-br from-purple-500 to-purple-600 rounded-xl flex items-center justify-center mb-3 group-hover:scale-110 transition-transform">
                  <Icon name="i-lucide-palette" class="w-6 h-6 text-white" />
                </div>
                <span class="text-sm font-medium text-slate-700">Customize</span>
              </button>

              <button class="flex flex-col items-center p-4 rounded-xl border border-slate-200/50 hover:border-primary-300 hover:bg-gradient-to-br hover:from-primary-50 hover:to-primary-100/50 transition-all duration-200 group">
                <div class="w-12 h-12 bg-gradient-to-br from-orange-500 to-orange-600 rounded-xl flex items-center justify-center mb-3 group-hover:scale-110 transition-transform">
                  <Icon name="i-lucide-image" class="w-6 h-6 text-white" />
                </div>
                <span class="text-sm font-medium text-slate-700">Add NFT</span>
              </button>

              <button class="flex flex-col items-center p-4 rounded-xl border border-slate-200/50 hover:border-primary-300 hover:bg-gradient-to-br hover:from-primary-50 hover:to-primary-100/50 transition-all duration-200 group">
                <div class="w-12 h-12 bg-gradient-to-br from-blue-500 to-blue-600 rounded-xl flex items-center justify-center mb-3 group-hover:scale-110 transition-transform">
                  <Icon name="i-lucide-bar-chart" class="w-6 h-6 text-white" />
                </div>
                <span class="text-sm font-medium text-slate-700">Analytics</span>
              </button>
            </div>
          </div>

          <!-- Links Management -->
          <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm">
            <div class="flex items-center justify-between mb-6">
              <h2 class="text-lg font-semibold text-slate-900">
                Your Links
              </h2>
              <UButton size="sm" icon="i-lucide-plus">
                Add Link
              </UButton>
            </div>

            <div class="space-y-4">
              <!-- Link Item -->
              <div class="flex items-center justify-between p-4 rounded-xl border border-slate-200/50 hover:border-slate-300 hover:bg-slate-50/50 transition-all duration-200">
                <div class="flex items-center gap-4">
                  <div class="w-12 h-12 bg-gradient-to-br from-blue-500 to-blue-600 rounded-xl flex items-center justify-center">
                    <Icon name="i-lucide-twitter" class="w-6 h-6 text-white" />
                  </div>
                  <div>
                    <h3 class="font-medium text-slate-900">
                      Twitter Profile
                    </h3>
                    <p class="text-sm text-slate-600">
                      @yourusername
                    </p>
                  </div>
                </div>
                <div class="flex items-center gap-3">
                  <div class="text-sm text-slate-600 bg-slate-100 px-2 py-1 rounded-full">
                    234 clicks
                  </div>
                  <div class="flex items-center gap-1">
                    <UButton variant="ghost" size="xs" icon="i-lucide-edit" />
                    <UButton variant="ghost" size="xs" icon="i-lucide-trash-2" />
                  </div>
                </div>
              </div>

              <!-- Link Item -->
              <div class="flex items-center justify-between p-4 rounded-xl border border-slate-200/50 hover:border-slate-300 hover:bg-slate-50/50 transition-all duration-200">
                <div class="flex items-center gap-4">
                  <div class="w-12 h-12 bg-gradient-to-br from-gray-700 to-gray-800 rounded-xl flex items-center justify-center">
                    <Icon name="i-lucide-github" class="w-6 h-6 text-white" />
                  </div>
                  <div>
                    <h3 class="font-medium text-slate-900">
                      GitHub Repository
                    </h3>
                    <p class="text-sm text-slate-600">
                      github.com/username/repo
                    </p>
                  </div>
                </div>
                <div class="flex items-center gap-3">
                  <div class="text-sm text-slate-600 bg-slate-100 px-2 py-1 rounded-full">
                    156 clicks
                  </div>
                  <div class="flex items-center gap-1">
                    <UButton variant="ghost" size="xs" icon="i-lucide-edit" />
                    <UButton variant="ghost" size="xs" icon="i-lucide-trash-2" />
                  </div>
                </div>
              </div>

              <!-- Link Item -->
              <div class="flex items-center justify-between p-4 rounded-xl border border-slate-200/50 hover:border-slate-300 hover:bg-slate-50/50 transition-all duration-200">
                <div class="flex items-center gap-4">
                  <div class="w-12 h-12 bg-gradient-to-br from-green-500 to-green-600 rounded-xl flex items-center justify-center">
                    <Icon name="i-lucide-globe" class="w-6 h-6 text-white" />
                  </div>
                  <div>
                    <h3 class="font-medium text-slate-900">
                      Personal Website
                    </h3>
                    <p class="text-sm text-slate-600">
                      yourwebsite.com
                    </p>
                  </div>
                </div>
                <div class="flex items-center gap-3">
                  <div class="text-sm text-slate-600 bg-slate-100 px-2 py-1 rounded-full">
                    89 clicks
                  </div>
                  <div class="flex items-center gap-1">
                    <UButton variant="ghost" size="xs" icon="i-lucide-edit" />
                    <UButton variant="ghost" size="xs" icon="i-lucide-trash-2" />
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Sidebar -->
        <div class="space-y-6">
          <!-- Profile Card -->
          <div class="bg-gradient-to-br from-white via-white to-primary-50/30 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm">
            <div class="text-center mb-6">
              <div class="w-20 h-20 bg-gradient-to-br from-primary-500 to-primary-600 rounded-full flex items-center justify-center mx-auto mb-4 ring-4 ring-primary-100">
                <Icon name="i-lucide-user" class="w-10 h-10 text-white" />
              </div>
              <h3 class="font-semibold text-slate-900 mb-1">
                @{{ $route.params.user }}
              </h3>
              <p class="text-sm text-slate-600">
                dotme.link/{{ $route.params.user }}
              </p>
            </div>

            <div class="space-y-3">
              <UButton variant="outline" block icon="i-lucide-settings">
                Edit Profile
              </UButton>
              <UButton variant="ghost" block icon="i-lucide-eye">
                View Public Page
              </UButton>
            </div>
          </div>

          <!-- Wallet Status -->
          <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm">
            <h3 class="font-semibold text-slate-900 mb-4">
              Wallet Status
            </h3>
            <div class="flex items-center gap-3 mb-4">
              <div class="w-10 h-10 bg-gradient-to-br from-primary-500 to-primary-600 rounded-full flex items-center justify-center">
                <Icon name="i-lucide-wallet" class="w-5 h-5 text-white" />
              </div>
              <div>
                <div class="font-medium text-slate-900 flex items-center gap-2">
                  Connected
                  <div class="w-2 h-2 bg-green-500 rounded-full" />
                </div>
                <div class="text-sm text-slate-600">
                  Polkadot Wallet
                </div>
              </div>
            </div>
            <div class="text-xs text-slate-600 mb-4 bg-slate-50 p-2 rounded-lg font-mono">
              5GrwvaEF5zXb26Fz9rcQpDWS57CtERHpNehXCPcNoHGKutQY
            </div>
            <UButton variant="outline" size="sm" block>
              Manage Wallet
            </UButton>
          </div>

          <!-- Recent Activity -->
          <div class="bg-white/80 backdrop-blur-sm rounded-xl p-6 border border-white/50 shadow-sm">
            <h3 class="font-semibold text-slate-900 mb-4">
              Recent Activity
            </h3>
            <div class="space-y-3">
              <div class="flex items-center gap-3 p-2 rounded-lg hover:bg-slate-50/50 transition-colors">
                <div class="w-2 h-2 bg-primary-600 rounded-full" />
                <div class="text-sm text-slate-600 flex-1">
                  Link clicked: Twitter Profile
                </div>
                <div class="text-xs text-slate-400">
                  2m ago
                </div>
              </div>
              <div class="flex items-center gap-3 p-2 rounded-lg hover:bg-slate-50/50 transition-colors">
                <div class="w-2 h-2 bg-blue-600 rounded-full" />
                <div class="text-sm text-slate-600 flex-1">
                  Page view from mobile
                </div>
                <div class="text-xs text-slate-400">
                  5m ago
                </div>
              </div>
              <div class="flex items-center gap-3 p-2 rounded-lg hover:bg-slate-50/50 transition-colors">
                <div class="w-2 h-2 bg-green-600 rounded-full" />
                <div class="text-sm text-slate-600 flex-1">
                  New link added: GitHub
                </div>
                <div class="text-xs text-slate-400">
                  1h ago
                </div>
              </div>
              <div class="flex items-center gap-3 p-2 rounded-lg hover:bg-slate-50/50 transition-colors">
                <div class="w-2 h-2 bg-slate-300 rounded-full" />
                <div class="text-sm text-slate-600 flex-1">
                  Profile updated
                </div>
                <div class="text-xs text-slate-400">
                  2h ago
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </UContainer>
  </div>
</template>
