<head>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Russo+One&display=swap" rel="stylesheet">
</head>

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
  
  <Navbar let:hidden let:toggle rounded color="form" class="z-50 fixed top-0 pt-3 md:pt-2 backdrop-blur-sm bg-black bg-transparent dark:backdrop-blur-sm	 dark:bg-transparent">
    <NavBrand href="/">
      <img src={smxlg} class="mr-4 ml-2 md:ml-1 md:mr-1 lg:mx-10 h-8 md:h-12 lg:h-15   dark:invert" alt="Logo"/>
      <span class="self-center whitespace-nowrap text-2xl lg:text-3xl font-semibold tracking-widest md:tracking-normal lg:tracking-widest">SMRT MRKT <span style="color:lime;">X</span></span>
    </NavBrand>
    <NavHamburger on:click={toggle} class=""/>
    <NavUl {hidden} class="font-semibold" >
      <NavLi href="/" active={false} on:click={() => { if (checkScreenSize()) toggle(); }} class="font-medium md:text-lg">Home</NavLi>
      <NavLi href="/products" on:click={() => { if (checkScreenSize()) toggle(); }} class="font-medium md:text-lg">Products</NavLi>
      <NavLi href="/services" on:click={() => { if (checkScreenSize()) toggle(); }} class="font-medium md:text-lg">Services</NavLi>
      <NavLi href="/digital" on:click={() => { if (checkScreenSize()) toggle(); }} class="font-medium md:text-lg">Digital</NavLi>
      <NavLi href="/bonus" on:click={() => { if (checkScreenSize()) toggle(); }} class="font-medium md:text-lg text-primary-customLime dark:text-primary-customLime">Bonus</NavLi>
    </NavUl>
  </Navbar>
  
  
  <div class="z-40 fixed top-20 md:top-20 right-0 flex justify-center m-2">
    <DarkMode class="text-black dark:text-white" />
  </div>
  
  <div class="mt-16"></div>
  
  
  <main class="my-1 p-2 border-y-4 border-black md:mt-20 md:text-lg md:p-10 md:text-center">
    <slot />
  </main>
  
  
  <Footer>
    
    <FooterLinkGroup aClass="font-style" ulClass="flex flex-wrap items-center mt-3 text-sm text-gray-500 dark:text-gray-400 sm:mt-0">
      <FooterLink href="/About">About</FooterLink>
      <FooterLink href="/PrivacyPolicy">Privacy Policy</FooterLink>
      <FooterLink href="/Licensing">Licensing</FooterLink>
      <FooterLink href="/Contact">Contact</FooterLink>
    </FooterLinkGroup>

    <FooterCopyright href="https://smx.tn" by="SMX" year={2023} aClass="text-black font-bold dark:text-white"/>

  </Footer>
  
  <style>

  </style>