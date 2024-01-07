<script>
import { Breadcrumb, BreadcrumbItem, AccordionItem, Accordion, GradientButton } from 'flowbite-svelte';
</script>

<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
    <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
    <BreadcrumbItem>Bonus</BreadcrumbItem>
</Breadcrumb>

<div class="justify-center items-center my-auto">
    <Accordion>
        <AccordionItem>
          <span slot="header">Passive Income</span>
          <p class="mb-2 text-gray-500 dark:text-gray-400">
            Passive income is any money earned in a manner that does not require too much effort.<br>
            There are several passive income generating ideas that require a lot of work, to begin with, like developing a blog or leasing property, but eventually, they earn money even when the owner is asleep.
            <br>
            <span class="flex justify-center items-center pt-5">
              <GradientButton color="greenToBlue">
                <a href="/bonus/passiveIncome" class="">get started</a></GradientButton>
            </span>
          </p>
        </AccordionItem>
        <AccordionItem transitionParams={{ duration: 2000 }}>
          <span slot="header">Direct Income</span>
          <p class="mb-2 text-gray-500 dark:text-gray-400">
            Direct income is the money that is received from doing tasks directly related to your business to make money.<br>
            Like Ads, Manual Faucets ...<br>
            <span class="flex justify-center items-center pt-5">
              <GradientButton color="greenToBlue">
                <a href="/bonus/directIncome" class="">get started</a></GradientButton>
            </span>
          </p>
        </AccordionItem>
        <AccordionItem transitionType="fade" transitionParams={{ duration: 1000 }}>
          <span slot="header">Other</span>
          <p class="mb-2 text-gray-500 dark:text-gray-400">Mining, Trading, Investing. Coming Soon ...</p>
        </AccordionItem>
      </Accordion>
</div>
