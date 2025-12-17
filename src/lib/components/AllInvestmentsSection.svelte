<script>
  const fundsLeft = [
    "Calamos Convertible Fund",
    "Calamos Growth Fund",
    "Calamos Market Neutral Income Fund",
    "Calamos Phineus Long/Short Fund",
    "Calamos Hedged Equity Fund",
    "Calamos Global Convertible Fund",
    "Calamos International Growth Fund",
    "Calamos Dividend Growth Fund",
    "Calamos Select Fund",
    "Calamos Global Dynamic Income Fund",
    "Calamos Strategic Total Return Fund",
    "Calamos Evolving World Growth Fund",
    "Calamos High Income Opportunities Fund",
    "Calamos Global Total Return Fund",
    "Calamos Timpani Small Cap Growth Fund",
    "Calamos Antetokounmpo Global Sustainable Equities Fund"
  ];

  const fundsRight = [
    "Calamos Convertible Opportunities Fund",
    "Calamos Dynamic Convertible & Income Fund",
    "Calamos Long/Short Equity & Dynamic Income Trust",
    "Calamos Strategic Total Return Fund",
    "Calamos Global Dynamic Income Fund",
    "Calamos Convertible and High Income Fund",
    "Calamos Alternative ETFs",
    "Calamos Hedged Equity ETF",
    "Calamos Market Neutral Income ETF",
    "Calamos Convertible ETF",
    "Calamos Short-Term Bond ETF",
    "Calamos Dynamic Convertible ETF",
    "Calamos Long/Short ETF",
    "Calamos Focus Growth ETF",
    "Calamos Dividend Growth ETF",
    "Calamos Select ETF"
  ];

  const categories = [
    "Convertible Strategies",
    "Liquid Alternatives",
    "Equity Strategies",
    "Fixed Income",
    "Multi-Asset",
    "ETFs",
    "Closed-End Funds"
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
        <h3 class="text-xl font-bold mb-4">Our Solutions</h3>
        <div class="text-gray-600 text-base leading-relaxed max-w-2xl mb-6">
          A comprehensive suite of investment solutions designed for RIAs and their high-net-worth clients. From our pioneering convertible securities strategies to innovative liquid alternatives, each solution reflects our commitment to institutional-grade quality and accessible sophistication.
        </div>
        <div class="flex flex-wrap gap-3 text-sm font-medium text-gray-500">
          {#each categories as category}
            <span class="hover:text-black cursor-pointer transition-colors">{category}</span>
            {#if category !== categories[categories.length - 1]}
              <span class="text-gray-300">•</span>
            {/if}
          {/each}
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-x-8 text-base font-medium leading-tight">
        <div class="space-y-2">
          {#each fundsLeft as fund}
            <div class="hover:text-gray-600 cursor-pointer transition-colors py-1">{fund}</div>
          {/each}
        </div>
        <div class="space-y-2">
          {#each fundsRight as fund}
            <div class="hover:text-gray-600 cursor-pointer transition-colors py-1">{fund}</div>
          {/each}
        </div>
      </div>

      <div class="mt-12 pt-8 border-t border-gray-300">
        <p class="text-sm text-gray-600 leading-relaxed max-w-3xl">
          <span class="font-bold">For Financial Advisors:</span> Each solution is designed with your practice in mind, offering institutional-grade strategies that help differentiate your services and meet the sophisticated needs of high-net-worth clients. Contact us to learn how Calamos can enhance your alternative investment offerings.
        </p>
      </div>
    </div>
  </div>
</section>
