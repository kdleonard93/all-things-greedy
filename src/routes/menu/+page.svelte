<script lang="ts">
    import { Card, Navbar, NavBrand, NavLi, NavUl } from 'flowbite-svelte';
  
    const sandwiches = [
      {
        name: 'Classic Club',
        description: 'Triple-decker with turkey, bacon, lettuce, and tomato',
        price: 12.99
      },
      {
        name: 'Veggie Delight',
        description: 'Fresh vegetables with homemade hummus',
        price: 10.99
      }
    ];
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

<main class="container mx-auto px-4 py-8">
  <div class="mx-auto px-4 py-8">
    <h1 class="text-3xl font-bold mb-6">Our Menu</h1>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      {#each sandwiches as sandwich}
        <Card>
          <h5 class="text-2xl font-bold tracking-tight text-gray-900 dark:text-white">
            {sandwich.name}
          </h5>
          <p class="font-normal text-gray-700 dark:text-gray-400">
            {sandwich.description}
          </p>
          <p class="font-bold text-lg">${sandwich.price}</p>
        </Card>
      {/each}
    </div>
  </div>
</main>
