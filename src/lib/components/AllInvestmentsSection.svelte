<script>
  const companiesLeft = [
    "15Five", "Acacia", "Accord", "Affirmed", "Afterpay", "Airvana", "Alteon", "Aluna", "Ambarella", "AMCC", 
    "Ampersand", "ApartmentList", "Apollo GraphQL", "ApplQ", "Apple", "Argon", "ArrowPoint", "Aruba", "August Health", 
    "Baselane", "Baya Systems", "Benny", "Bonsai", "Broadband Access", "Bugsnag", "Camiant", "Canva", "Care.com", 
    "Cascade", "Centaur Labs", "Chameleon", "CloudBees", "CloudSwitch", "CloudZero", "CommonGround", "Concerto", 
    "Conductor", "Confer", "Copper Mountain", "Cosmos", "Courier", "CTRL Labs", "Earnin", "Educative", "Emerge Tools", 
    "Empirix", "Fabletics", "FedEx", "Fini", "Fivetran", "Flex", "Flock Safety", "General Medicine", "Gentrace", 
    "Gilt Groupe", "GOAT", "GrabCAD", "Hashboard", "Headlight", "Hookdeck", "Hubspot", "Infinity AI", "Inflection", 
    "JBoss", "Keeper Tax", "Kolide", "Lam Research", "Lever", "Lightforce", "Lightmatter", "LM Studio", "LogRocket"
  ];

  const companiesRight = [
    "Luma AI", "Markforged", "Mashgin", "Meadow", "Mesa", "Meshcapade", "Mevo", "Mudflap", "Namely", "Netezza", 
    "nference", "Nubis", "Objective", "Oculus", "OmniML", "ONDisplay", "OpenPages", "Openwave", "Owl Labs", "Parabola", 
    "PayRange", "Pingo", "Pixcel", "Plexxi", "Polyvore", "Postmates", "PostPath", "Poynt", "Prominet", "QPID", 
    "Quora", "Rainforest", "Redstone", "Relace", "Reshop", "Salient", "Salsify", "SanDisk", "Sesame", "Side", 
    "Sieve", "Sila", "SilverStream", "SiTera", "Smartcat", "Sonus", "Splitwise", "Spring Tide", "Starent", "Steadily", 
    "Suno", "Sycamore", "Tabblo", "Taxa", "Tealeaf", "Teammates", "Tencor", "The Echo Nest", "The Ladders", 
    "Tivoli Software", "Trisk Bio", "Turnstone", "Unidesk", "Veritas", "Vermeer", "WatchGuard", "Winphoria", "Xilinx", 
    "Xtalic", "Zendesk", "Zest AI", "Zong"
  ];
</script>

<section class="py-20 px-6 md:px-12">
  <div class="flex flex-col md:flex-row">
    <!-- Left Spacer -->
    <div class="w-full md:w-1/4 pr-8 hidden md:block">
      <!-- Empty to align with right column of previous sections -->
    </div>

    <!-- Right Column Content -->
    <div class="w-full md:w-3/4">
      <div class="mb-12">
        <div class="flex space-x-4 text-xl font-bold mb-4">
          <span class="text-black">All,</span>
          <span class="text-gray-400">Acquired,</span>
          <span class="text-gray-400">IPO</span>
        </div>
        <div class="text-gray-400 text-lg leading-relaxed max-w-2xl">
          AI, B2B, Consumer, FinTech, Frontier, HealthTech, Infrastructure, Semiconductors
        </div>
      </div>

      <div class="grid grid-cols-2 gap-x-8 text-lg font-medium leading-tight">
        <div class="space-y-1">
          {#each companiesLeft as company}
            <div class="hover:text-blue-600 cursor-pointer transition-colors">{company}</div>
          {/each}
        </div>
        <div class="space-y-1">
          {#each companiesRight as company}
            <div class="hover:text-blue-600 cursor-pointer transition-colors">{company}</div>
          {/each}
        </div>
      </div>
    </div>
  </div>
</section>
