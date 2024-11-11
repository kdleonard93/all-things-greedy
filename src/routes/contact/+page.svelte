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
    <h1 class="text-3xl font-bold mb-6">Let us Cater!</h1>
    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <h3>Phone: 111-222-3333</h3>
        <h3>Email: email@gmail.com</h3>
    </div>
  </div>
</main>