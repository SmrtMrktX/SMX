<script>
    import { Breadcrumb, BreadcrumbItem } from 'flowbite-svelte';
    import Loading from "$lib/Components/Loading.svelte";
</script>
    
<Breadcrumb aria-label="Default breadcrumb example" class="my-4">
    <BreadcrumbItem href="/" home>Home</BreadcrumbItem>
    <BreadcrumbItem>Digital</BreadcrumbItem>
</Breadcrumb>


<Loading />