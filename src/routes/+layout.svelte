<script>
    import "../app.pcss";
    import smxlg from "$lib/img/smxlg.png"
    import { DarkMode } from 'flowbite-svelte';
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterLink } from 'flowbite-svelte';

    // Check screen size
    function checkScreenSize() {
      return window.innerWidth <= 768; // Adjust the value as needed
    }

  </script>
  
  <Navbar let:hidden let:toggle rounded color="form" class="fixed top-0  backdrop-blur-sm bg-black bg-transparent dark:backdrop-blur-sm	 dark:bg-transparent">
    <NavBrand href="/">
      <img src={smxlg} class="mr-3 h-9 sm:h-11" alt="Logo"/>
      <span class="self-center whitespace-nowrap font-bold italic text-2xl sm:text-3xl">SMRT MRKT <span style="color:lime;">X</span></span>
    </NavBrand>
    <NavHamburger on:click={toggle} class=""/>
    <NavUl {hidden} class="font-semibold" >
      <NavLi href="/" active={false} on:click={() => { if (checkScreenSize()) toggle(); }} class="md:text-lg">Home</NavLi>
      <NavLi href="/about" on:click={() => { if (checkScreenSize()) toggle(); }} class="md:text-lg">About</NavLi>
      <NavLi href="/services" on:click={() => { if (checkScreenSize()) toggle(); }} class="md:text-lg">Services</NavLi>
      <NavLi href="/pricing" on:click={() => { if (checkScreenSize()) toggle(); }} class="md:text-lg">Pricing</NavLi>
      <NavLi href="/bonus" on:click={() => { if (checkScreenSize()) toggle(); }} class="md:text-lg font-bold text-primary-customLime dark:text-primary-customLime">Bonus</NavLi>
    </NavUl>
  </Navbar>
  
  
  <div class="fixed top-16 md:top-20 right-0 flex justify-center m-2">
    <DarkMode class="text-black dark:text-white" />
  </div>
  
  <div class="mt-16"></div>
  
  
  <main class="my-1 p-2 border-y-4 border-black md:mt-20 md:text-lg md:p-10 md:text-center">
    <slot />
  </main>
  
  
  <Footer>
    
    <FooterLinkGroup ulClass="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
      <FooterLink href="/">About</FooterLink>
      <FooterLink href="/">Privacy Policy</FooterLink>
      <FooterLink href="/Licensing">Licensing</FooterLink>
      <FooterLink href="/">Contact</FooterLink>
    </FooterLinkGroup>

    <FooterCopyright href="https://smx.tn" by="SMX" year={2023} aClass="text-black font-bold dark:text-white"/>

  </Footer>
  
  <style>
  
  </style>