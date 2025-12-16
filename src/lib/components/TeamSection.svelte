<script>
  const team = [
    {
      name: "Antonio Rodriguez",
      role: "AI, Frontier",
      investments: "Asana, Luma Labs, Markforged, Owl Labs, Sesame, Suno, Trisk Bio",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=AR"
    },
    {
      name: "Dana Stalder",
      role: "FinTech, B2B",
      investments: "ApartmentList, Baselane, Earnin, Flexible Finance, Mudflap, Side, Steadily, Zest AI",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=DS"
    },
    {
      name: "Ilya Sukhar",
      role: "AI, Infrastructure",
      investments: "August Health, Chameleon, Fivetran, Flock Safety, Mashgin, Parabola, Sieve",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=IS"
    },
    {
      name: "Kojo Osei",
      role: "AI, Infrastructure",
      investments: "Hookdeck, Ampersand, LM Studio",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=KO"
    },
    {
      name: "Matt Brown",
      role: "FinTech, B2B",
      investments: "Rainforest, Meadow, Benny",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=MB"
    },
    {
      name: "Patrick Malatack",
      role: "Infrastructure",
      investments: "Courier, Hookdeck, Ampersand, Salient, Fini",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=PM"
    },
    {
      name: "Stan Reiss",
      role: "Semiconductors",
      investments: "Baya Systems, Centaur Labs, Lightforce, Lightmatter, LogRocket, Nabis, Xtalic",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=SR"
    },
    {
      name: "TJ Parker",
      role: "HealthTech",
      investments: "General Medicine, Headlight, Mevo",
      image: "https://placehold.co/400x500/e5e5e5/a3a3a3?text=TP"
    }
  ];
</script>

<section id="team" class="py-20 px-6 md:px-12 border-t border-gray-300">
  <div class="flex flex-col md:flex-row">
    <!-- Left Column -->
    <div class="w-full md:w-1/4 pr-8 mb-12 md:mb-0">
      <h2 class="text-xl font-bold mb-8">Team</h2>
      <p class="text-2xl md:text-3xl font-medium leading-tight max-w-xs">
        A close-knit team of former founders and company builders. We are selective in our investments and generous with our time.
      </p>
    </div>

    <!-- Right Column -->
    <div class="w-full md:w-3/4">
      <div class="flex space-x-6 mb-8 text-lg border-b border-gray-300">
        <button class="font-bold text-black border-b-2 border-black pb-4 px-1 -mb-[1px]">Investing</button>
        <button class="text-gray-400 hover:text-gray-600 transition-colors pb-4 px-1">Operations</button>
        <button class="text-gray-400 hover:text-gray-600 transition-colors pb-4 px-1">Emeritus</button>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-x-8 gap-y-12">
        {#each team as member}
          <div class="group cursor-pointer">
            <div class="aspect-[4/5] bg-gray-200 mb-4 overflow-hidden">
              <img src={member.image} alt={member.name} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
            </div>
            <h3 class="font-bold text-lg">{member.name}</h3>
            <p class="text-gray-500 text-sm mb-3">{member.role}</p>
            <p class="text-xs leading-relaxed mb-4 h-16 overflow-hidden">{member.investments}</p>
            <div class="flex space-x-3 text-gray-400 text-xs">
               <!-- Icons placeholders -->
               <span>LI</span>
               <span>X</span>
            </div>
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
