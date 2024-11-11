<script lang="ts">
    import {Navbar, NavBrand, NavLi, NavUl } from 'flowbite-svelte';

  </script>

<Navbar let:hidden let:toggle>
    <NavBrand href="/">
      <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
        All Things Greedy
      </span>
    </NavBrand>
    <NavUl {hidden}>
      <NavLi href="/">Home</NavLi>
      <NavLi href="/menu">Menu</NavLi>
      <NavLi href="/about">About</NavLi>
      <NavLi href="/contact">Contact</NavLi>
    </NavUl>
  </Navbar>
  
  <main class="container mx-auto px-4 py-8 flex justify-center">
  <div class="mx-auto px-4 py-8">
    <h1 class="text-3xl font-bold mb-6">About My Business</h1>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <p>Lorem ipsum odor amet, consectetuer adipiscing elit. Sit conubia accumsan sit aptent natoque arcu. Aptent et accumsan potenti vulputate rhoncus nullam. Curae viverra nunc duis quam in felis nostra massa. Rhoncus nibh varius etiam posuere egestas condimentum maximus sem. Scelerisque sollicitudin gravida finibus; vehicula eu dui. Faucibus congue cursus eros vestibulum penatibus amet. Primis nisl augue ultrices taciti tincidunt volutpat dignissim.</p>

        <p>Justo dolor fames torquent dictum vitae cras vitae donec. Est nunc enim urna penatibus nam iaculis mus augue ante. Praesentsenectus duis potenti, magnis tortor sollicitudin augue pulvinar. Potenti lacinia justo id metus integer. Penatibus eratfeugiat pellentesque metus aptent pretium sociosqu habitant. Sed a ut odio dui montes curabitur netus cubilia inceptos.</p>
    </div>
  </div>
</main>

