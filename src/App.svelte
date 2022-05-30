<script>
    import Settings from "./Setting.svelte";
    import Dashboard from "./Dashboard.svelte";
    import Profile from "./Profile.svelte";
</script>

<main>
    <Settings />
    <Dashboard />
    <Profile />
</main>

<style>
    main {
        display: grid;
        grid-template-columns: 122px 1fr 329px;
        grid-template-areas: "settings main profile";
    }
</style>
