<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import ComingSoon from "$lib/Components/ComingSoon.svelte";
</script>
    
<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
    <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
    <BreadcrumbItem>Products</BreadcrumbItem>
</Breadcrumb>


<ComingSoon />