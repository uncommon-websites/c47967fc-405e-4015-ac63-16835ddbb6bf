<script>
  const leadership = [
    {
      name: "John P. Calamos Sr.",
      role: "Founder & Global CIO",
      description: "Pioneered convertible securities management in 1977. Four decades transforming a boutique firm into a $46B global asset manager.",
      image: "/generated/image-confident-senior-executive-in-his-70s-at-1766009994896-0.webp"
    }
  ];
</script>

<section id="leadership" class="py-20 px-6 md:px-12 border-t border-gray-300">
  <div class="flex flex-col md:flex-row">
    <!-- Left Column -->
    <div class="w-full md:w-1/4 pr-8 mb-12 md:mb-0">
      <h2 class="text-xl font-bold mb-8">Leadership</h2>
      <p class="text-2xl md:text-3xl font-medium leading-tight max-w-xs">
        Innovation over imitation. Execution over trends. Nearly five decades of disciplined risk management.
      </p>
    </div>

    <!-- Right Column -->
    <div class="w-full md:w-3/4">
      <div class="mb-12">
        <h3 class="text-xl font-bold mb-6">Our Founder</h3>
        <div class="max-w-2xl">
          {#each leadership as member}
            <div class="group cursor-pointer mb-12">
              <div class="flex flex-col md:flex-row gap-8">
                <div class="w-full md:w-1/3">
                  <div class="aspect-[4/5] bg-gray-200 overflow-hidden">
                    <img src={member.image} alt={member.name} class="w-full h-full object-cover grayscale group-hover:grayscale-0 transition-all duration-500" />
                  </div>
                </div>
                <div class="w-full md:w-2/3 flex flex-col justify-center">
                  <h3 class="font-bold text-2xl mb-2">{member.name}</h3>
                  <p class="text-gray-500 text-base mb-4">{member.role}</p>
                  <p class="text-base leading-relaxed">{member.description}</p>
                </div>
              </div>
            </div>
          {/each}
        </div>
      </div>

      <div class="border-t border-gray-300 pt-12">
        <h3 class="text-xl font-bold mb-6">Our Philosophy</h3>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-base leading-relaxed">
          <div>
            <h4 class="font-bold mb-3">Heritage & Innovation</h4>
            <p class="text-gray-700">Founded in 1977 as a boutique convertible securities specialist, we've evolved into a diversified global investment firm while maintaining our core discipline and expertise.</p>
          </div>
          <div>
            <h4 class="font-bold mb-3">Risk Management First</h4>
            <p class="text-gray-700">Our approach centers on disciplined risk management and risk-adjusted returns, bringing institutional-grade strategies to a broader market.</p>
          </div>
          <div>
            <h4 class="font-bold mb-3">Client Excellence</h4>
            <p class="text-gray-700">We serve RIAs and their high-net-worth clients with the same sophistication and attention previously reserved for institutional investors.</p>
          </div>
          <div>
            <h4 class="font-bold mb-3">Trend Creation</h4>
            <p class="text-gray-700">We don't follow trends, we create them. Our proactive approach and innovation-first mindset drive market leadership.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
