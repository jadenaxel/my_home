<script>
    const imageLink = [
        "/images/icons/settings/chart.svg",
        "/images/icons/settings/union.svg",
        "/images/icons/settings/bookmark.svg",
        "/images/icons/settings/settings.svg",
    ];
</script>

<div class="settings">
    <img class="settings-title" src="/images/logo.svg" alt="Logo" />
    <div class="settings-link">
        {#each imageLink as image}
            <img src={image} alt="Settings" class="settings-link-item" />
        {/each}
    </div>
</div>

<style>
    .settings {
        grid-area: settings;
        background-color: #000;
        min-height: 100vh;
        padding: 25px 10px;
    }
    .settings-title {
        cursor: pointer;
        margin-bottom: 64px;
    }
    .settings-link {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .settings-link-item {
        margin-bottom: 70px;
        cursor: pointer;
    }
    .settings-link-item:last-child {
        margin-bottom: 0;
    }
</style>
