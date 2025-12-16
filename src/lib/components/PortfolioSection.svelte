<script>
  const investments = [
    { name: "Afterpay", logo: "AP" },
    { name: "Apple", logo: "" },
    { name: "Canva", logo: "Ca" },
    { name: "Fivetran", logo: "Fi" },
    { name: "Flex", logo: "fl" },
    { name: "Flock Safety", logo: "FS" },
    { name: "GOAT", logo: "GO" },
    { name: "Hubspot", logo: "Hb" },
    { name: "Luma AI", logo: "Lu" },
    { name: "Oculus", logo: "Oc" },
    { name: "Suno", logo: "Su" },
    { name: "Zendesk", logo: "Ze" },
  ];
</script>

<section id="portfolio" class="py-20 px-6 md:px-12 border-t border-gray-300">
  <div class="flex flex-col md:flex-row">
    <!-- Left Column -->
    <div class="w-full md:w-1/4 pr-8 mb-12 md:mb-0">
      <h2 class="text-xl font-bold mb-8">Portfolio</h2>
      <p class="text-2xl md:text-3xl font-medium leading-tight max-w-xs">
        Challengers, contrarians, risk-takers, and status-quo-breakers. Our portfolio companies are built by founders with deep technical expertise and a specific vision of the future.
      </p>
    </div>

    <!-- Right Column -->
    <div class="w-full md:w-3/4">
      <h3 class="text-xl font-bold mb-8">Select Investments</h3>

      <div class="grid grid-cols-2 md:grid-cols-3 gap-4">
        {#each investments as company}
          <div class="aspect-square bg-[#dcdcdc] flex flex-col justify-between p-4 hover:bg-[#d0d0d0] transition-colors cursor-pointer group">
            <div class="flex-grow flex items-center justify-center">
                <!-- Logo Placeholder -->
                <span class="text-4xl font-bold opacity-50 group-hover:opacity-100 transition-opacity">{company.logo}</span>
            </div>
            <span class="text-xs font-medium">{company.name}</span>
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
