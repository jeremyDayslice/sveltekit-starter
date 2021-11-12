<script>
    export let name = "Timmy";

    let menuItems = [
        {
            label: 'Home',
            active: true,
         },
         {
            label: 'About',
            active: false,
         },
         {
            label: 'FAQ',
            active: false,
         }
    ]

    const setActive = (index) => {
        debugger
        menuItems[index].active = true;
    }
</script>

<h3>{name}</h3>
<ul>
    {#each menuItems as menuItem, index}
        <li class:active={menuItem.active} on:click={( () => setActive(index))} >{menuItem}</li>
    {/each}
</ul>

<style>
    .active {
        font-weight: bold; color: #47aa88;
    }
</style>