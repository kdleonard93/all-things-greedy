<script lang="ts">
    import { Button, Navbar, NavBrand, NavLi, NavUl } from 'flowbite-svelte';
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
    <div class="text-center">
      <h1 class="text-4xl font-bold mb-4">Welcome to All Things Greedy</h1>
      <p class="mb-6">Crafting the perfect sandwich for every taste</p>
      <Button href="/menu">View Our Menu</Button>
    </div>
  </main>