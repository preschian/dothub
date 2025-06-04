<template>
  <!-- Hero Section -->
  <section class="pt-20 pb-32">
    <UContainer>
      <div class="max-w-4xl mx-auto text-center">
        <div class="inline-flex items-center gap-2 bg-primary-50 text-primary-700 px-4 py-2 rounded-full text-sm font-medium mb-8">
          <Icon name="i-lucide-sparkles" class="w-4 h-4" />
          Built on Polkadot Blockchain
        </div>

        <h1 class="text-5xl md:text-7xl font-bold text-slate-900 mb-8 tracking-tight">
          Your links,
          <br>
          <span class="text-primary-600">decentralized</span>
        </h1>

        <p class="text-xl text-slate-600 mb-12 max-w-2xl mx-auto leading-relaxed">
          Create a beautiful link page that you truly own. Built on blockchain technology for ultimate security and control.
        </p>

        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <UButton size="lg" class="px-8 py-3">
            Create Your Page
          </UButton>
          <UButton size="lg" variant="ghost" class="px-8 py-3">
            View Example
            <Icon name="i-lucide-arrow-right" class="w-4 h-4 ml-2" />
          </UButton>
        </div>
      </div>
    </UContainer>
  </section>

  <!-- Features Section -->
  <section class="bg-slate-50 py-24">
    <UContainer>
      <div class="max-w-3xl mx-auto text-center mb-20">
        <h2 class="text-3xl md:text-4xl font-bold text-slate-900 mb-6">
          Everything you need
        </h2>
        <p class="text-lg text-slate-600">
          Simple, powerful, and completely under your control
        </p>
      </div>

      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
        <!-- Feature 1 -->
        <div class="bg-white p-8 rounded-2xl">
          <div class="w-12 h-12 bg-primary-100 rounded-xl flex items-center justify-center mb-6">
            <Icon name="i-lucide-shield" class="w-6 h-6 text-primary-600" />
          </div>
          <h3 class="text-lg font-semibold text-slate-900 mb-3">
            Blockchain Secured
          </h3>
          <p class="text-slate-600">
            Your page is stored on Polkadot blockchain, ensuring permanent ownership and security.
          </p>
        </div>

        <!-- Feature 2 -->
        <div class="bg-white p-8 rounded-2xl">
          <div class="w-12 h-12 bg-primary-100 rounded-xl flex items-center justify-center mb-6">
            <Icon name="i-lucide-paintbrush" class="w-6 h-6 text-primary-600" />
          </div>
          <h3 class="text-lg font-semibold text-slate-900 mb-3">
            Custom Design
          </h3>
          <p class="text-slate-600">
            Choose from beautiful themes or create your own unique design that reflects your brand.
          </p>
        </div>

        <!-- Feature 3 -->
        <div class="bg-white p-8 rounded-2xl">
          <div class="w-12 h-12 bg-primary-100 rounded-xl flex items-center justify-center mb-6">
            <Icon name="i-lucide-bar-chart" class="w-6 h-6 text-primary-600" />
          </div>
          <h3 class="text-lg font-semibold text-slate-900 mb-3">
            Analytics
          </h3>
          <p class="text-slate-600">
            Track clicks, views, and engagement with detailed analytics and insights.
          </p>
        </div>

        <!-- Feature 4 -->
        <div class="bg-white p-8 rounded-2xl">
          <div class="w-12 h-12 bg-primary-100 rounded-xl flex items-center justify-center mb-6">
            <Icon name="i-lucide-wallet" class="w-6 h-6 text-primary-600" />
          </div>
          <h3 class="text-lg font-semibold text-slate-900 mb-3">
            Web3 Native
          </h3>
          <p class="text-slate-600">
            Connect your wallet and manage everything on-chain with full transparency.
          </p>
        </div>

        <!-- Feature 5 -->
        <div class="bg-white p-8 rounded-2xl">
          <div class="w-12 h-12 bg-primary-100 rounded-xl flex items-center justify-center mb-6">
            <Icon name="i-lucide-globe" class="w-6 h-6 text-primary-600" />
          </div>
          <h3 class="text-lg font-semibold text-slate-900 mb-3">
            Always Online
          </h3>
          <p class="text-slate-600">
            Your page is accessible 24/7 with 99.9% uptime guaranteed by the blockchain.
          </p>
        </div>

        <!-- Feature 6 -->
        <div class="bg-white p-8 rounded-2xl">
          <div class="w-12 h-12 bg-primary-100 rounded-xl flex items-center justify-center mb-6">
            <Icon name="i-lucide-users" class="w-6 h-6 text-primary-600" />
          </div>
          <h3 class="text-lg font-semibold text-slate-900 mb-3">
            Community
          </h3>
          <p class="text-slate-600">
            Join thousands of creators building their presence on the decentralized web.
          </p>
        </div>
      </div>
    </UContainer>
  </section>

  <!-- How It Works -->
  <section class="py-24">
    <UContainer>
      <div class="max-w-3xl mx-auto text-center mb-20">
        <h2 class="text-3xl md:text-4xl font-bold text-slate-900 mb-6">
          Get started in minutes
        </h2>
        <p class="text-lg text-slate-600">
          Three simple steps to create your decentralized link page
        </p>
      </div>

      <div class="max-w-4xl mx-auto">
        <div class="grid md:grid-cols-3 gap-12">
          <!-- Step 1 -->
          <div class="text-center">
            <div class="w-16 h-16 bg-primary-600 text-white rounded-2xl flex items-center justify-center mx-auto mb-6 text-xl font-bold">
              1
            </div>
            <h3 class="text-xl font-semibold text-slate-900 mb-4">
              Connect Wallet
            </h3>
            <p class="text-slate-600">
              Connect your Polkadot wallet to authenticate and secure your identity on the blockchain.
            </p>
          </div>

          <!-- Step 2 -->
          <div class="text-center">
            <div class="w-16 h-16 bg-primary-600 text-white rounded-2xl flex items-center justify-center mx-auto mb-6 text-xl font-bold">
              2
            </div>
            <h3 class="text-xl font-semibold text-slate-900 mb-4">
              Design Page
            </h3>
            <p class="text-slate-600">
              Add your links, choose a theme, and customize your page to match your style and brand.
            </p>
          </div>

          <!-- Step 3 -->
          <div class="text-center">
            <div class="w-16 h-16 bg-primary-600 text-white rounded-2xl flex items-center justify-center mx-auto mb-6 text-xl font-bold">
              3
            </div>
            <h3 class="text-xl font-semibold text-slate-900 mb-4">
              Share & Track
            </h3>
            <p class="text-slate-600">
              Share your unique URL and track performance with built-in analytics and insights.
            </p>
          </div>
        </div>
      </div>
    </UContainer>
  </section>

  <!-- CTA Section -->
  <section class="bg-slate-900 py-24">
    <UContainer>
      <div class="text-center">
        <div class="max-w-3xl mx-auto">
          <h2 class="text-3xl md:text-4xl font-bold text-white mb-6">
            Own your digital presence
          </h2>
          <p class="text-xl text-slate-300 mb-10">
            Join the decentralized web and take control of your links, data, and digital identity.
          </p>
          <div class="flex flex-col sm:flex-row gap-4 justify-center">
            <UButton size="lg" class="px-8 py-3">
              Get Started Free
            </UButton>
            <UButton size="lg" variant="outline" class="px-8 py-3 border-slate-600 text-slate-300 hover:bg-slate-800">
              Learn More
            </UButton>
          </div>
        </div>
      </div>
    </UContainer>
  </section>
</template>
