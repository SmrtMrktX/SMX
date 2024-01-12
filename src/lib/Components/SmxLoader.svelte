<script>

        import smxloader from "$lib/img/smxloader.png";

        // Array of names
        const names = ["TRUST", "PRIVACY", "SECURITY"];

        // Function to choose a random name
        function chooseRandomName() {
        const randomIndex = Math.floor(Math.random() * names.length);
        return names[randomIndex];
        }

        // Example usage
        const randomName = chooseRandomName();
        // console.log("Randomly chosen name: " + randomName);
</script>




<div class="justify-center items-center text-center m-auto">
        
        <img src={smxloader} class="mx-auto h-12  md:h-14 lg:h-16  rounded-md   animate-bounce dark:invert" alt="SMX Logo"/>
        <h1 style="font-family: 'Russo One', sans-serif;font-weight:900;" class="text-xl animate-pulse mt-10 tracking-widest">{randomName}</h1>
</div>