<script>
  const strategies = [
    { name: "Convertible Securities", icon: "CS", description: "Our heritage strategy" },
    { name: "Liquid Alternatives", icon: "LA", description: "3rd largest in US" },
    { name: "Multi-Strategy", icon: "MS", description: "Diversified approach" },
    { name: "Risk-Adjusted Returns", icon: "RA", description: "Core discipline" },
    { name: "Global Equities", icon: "GE", description: "International reach" },
    { name: "Fixed Income", icon: "FI", description: "Balanced portfolios" }
  ];
</script>

<section id="approach" class="py-20 px-6 md:px-12 border-t border-gray-300">
  <div class="flex flex-col md:flex-row">
    <!-- Left Column -->
    <div class="w-full md:w-1/4 pr-8 mb-12 md:mb-0">
      <h2 class="text-xl font-bold mb-8">Our Approach</h2>
      <p class="text-2xl md:text-3xl font-medium leading-tight max-w-xs">
        Institutional-grade strategies built on convertible securities expertise and liquid alternatives innovation. Accessible, sophisticated, disciplined.
      </p>
    </div>

    <!-- Right Column -->
    <div class="w-full md:w-3/4">
      <h3 class="text-xl font-bold mb-8">Investment Strategies</h3>

      <div class="grid grid-cols-2 md:grid-cols-3 gap-4 mb-12">
        {#each strategies as strategy}
          <div class="aspect-square bg-[#0a0a0a] flex flex-col justify-between p-6 hover:bg-[#171717] transition-colors cursor-pointer group">
            <div class="flex-grow flex items-center justify-center">
                <span class="text-3xl font-bold text-white opacity-80 group-hover:opacity-100 transition-opacity">{strategy.icon}</span>
            </div>
            <div class="text-white">
              <span class="text-sm font-bold block mb-1">{strategy.name}</span>
              <span class="text-xs text-gray-400">{strategy.description}</span>
            </div>
          </div>
        {/each}
      </div>

      <div class="border-t border-gray-300 pt-12">
        <h3 class="text-xl font-bold mb-6">Our Competitive Edge</h3>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-6 text-base">
          <div class="space-y-3">
            <div class="flex items-start">
              <span class="font-bold mr-3">•</span>
              <p><span class="font-bold">$46 Billion AUM</span> — Scale and stability built over nearly five decades</p>
            </div>
            <div class="flex items-start">
              <span class="font-bold mr-3">•</span>
              <p><span class="font-bold">$20B+ in Alternatives</span> — Third-largest liquid alternatives provider in the US</p>
            </div>
            <div class="flex items-start">
              <span class="font-bold mr-3">•</span>
              <p><span class="font-bold">Convertible Securities Leader</span> — Largest manager in the United States</p>
            </div>
          </div>
          <div class="space-y-3">
            <div class="flex items-start">
              <span class="font-bold mr-3">•</span>
              <p><span class="font-bold">Since 1977</span> — Nearly 50 years of proven track record and expertise</p>
            </div>
            <div class="flex items-start">
              <span class="font-bold mr-3">•</span>
              <p><span class="font-bold">RIA-Focused</span> — Designed for advisors serving high-net-worth clients</p>
            </div>
            <div class="flex items-start">
              <span class="font-bold mr-3">•</span>
              <p><span class="font-bold">Innovation First</span> — Creating trends, not following them</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
