<script>
    // Components
    import NavigationBar from "$lib/NavigationBar/NavigationBar.svelte";
    import NavigationMargin from "$lib/NavigationBar/NavMargin.svelte";
    import LoadingSpinner from "$lib/LoadingSpinner/Spinner.svelte";
</script>

<svelte:head>
    <title>ElectraMod - Loading</title>
    <meta name="title" content="ElectraMod - Home" />
    <meta property="og:title" content="ElectraMod - Home" />
    <meta property="twitter:title" content="ElectraMod - Home">
    <meta name="description" content="The area where featured projects and community stuff & info is shown.">
    <meta property="twitter:description" content="The area where featured projects and community stuff & info is shown.">
    <meta property="og:url" content="https://electramod-home.vercel.app/">
    <meta property="twitter:url" content="https://electramod-home.vercel.app/">
</svelte:head>

<NavigationBar />

<div class="main">
    <NavigationMargin />

    <div class="box">
        <LoadingSpinner />
    </div>
</div>

<style>
    * {
        font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    }

    .main {
        position: absolute;
        left: 0px;
        top: 0px;
        width: 100%;
        min-width: 1000px;
    }
    .box {
        margin-top: 32px;
        width: 100%;
        display: flex;
        flex-direction: column;
        align-items: center;
    }
</style>
