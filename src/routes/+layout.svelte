<script>
    import "../app.pcss";
    import smxlg from "$lib/img/smxlg.png"
    import { DarkMode } from 'flowbite-svelte';
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
    import { Footer, FooterCopyright, FooterLinkGroup, FooterLink } from 'flowbite-svelte';
  </script>
  
  <Navbar let:hidden let:toggle rounded color="form" class="fixed top-0  backdrop-blur-sm bg-black bg-transparent dark:backdrop-blur-sm	 dark:bg-transparent">
    <NavBrand href="/">
      <img src={smxlg} class="mr-3 h-9 sm:h-11" alt="Logo"/>
      <span class="self-center whitespace-nowrap text-2xl sm:text-3xl font-bold ">SMRT MRKT X</span>
    </NavBrand>
    <NavHamburger on:click={toggle}/>
    <NavUl {hidden} >
      <NavLi href="/" active={false}>Home</NavLi>
      <NavLi href="/about">About</NavLi>
      <NavLi href="/services">Services</NavLi>
      <NavLi href="/pricing">Pricing</NavLi>
      <NavLi href="/contact">Contact</NavLi>
    </NavUl>
  </Navbar>
  
  
  <div class="fixed top-16 right-0 flex justify-center m-2">
    <DarkMode class="text-black dark:text-white" />
  </div>
  
  <div class="mt-16"></div>
  
  
  <main class="font-mono my-1 p-2 bg-customColorW text-customColorD dark:bg-customColorD dark:text-customColorW">
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