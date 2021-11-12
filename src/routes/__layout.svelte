<script>
    import HeaderMenu from "$lib/HeaderMenu.svelte";

    let favNumber = 4+8
</script>

<HeaderMenu name={favNumber}></HeaderMenu>

<slot></slot>