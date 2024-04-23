<script>import "../app.pcss";

import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
    import { Dropdown, DropdownItem } from 'flowbite-svelte';
</script>
    
    <Navbar let:NavContainer color="primary">
        <NavContainer class="border px-5 py-2 rounded-lg bg-white dark:bg-gray-600">
    <NavBrand href="/">
      <img src="" class="me-3 h-6 sm:h-9" alt="MYfood_logo" />
      <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">My_Recipes</span>
    </NavBrand>
    <NavHamburger  />
    
    <NavUl>
        <NavLi href="/">Home</NavLi>
        <NavLi class="cursor-pointer">Recipies</NavLi>

            <Dropdown class="w-28 z-20">
                <DropdownItem href="Breakfast">Breakfast</DropdownItem>
                <DropdownItem href="Curries">Curries</DropdownItem>
                <DropdownItem href="Rice">Rice</DropdownItem>
                <DropdownItem href="snacks">Snacks</DropdownItem>
                 <DropdownItem href ="Soup">Soup</DropdownItem>
                
            </Dropdown>

        
         <NavLi href="/docs/components/navbar">About</NavLi>
        <NavLi href="/contact">Contact</NavLi>
    </NavUl>
      
</NavContainer>
</Navbar>

<slot />

