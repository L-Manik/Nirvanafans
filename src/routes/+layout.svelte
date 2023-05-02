<div class="main-wrapper">
    <div class="sidebar"></div>
    <div class="content">
        <slot/>
    </div>
</div>

<style>
    :global(*) {
        margin: 0;
        padding: 0;
    }
    :global(html, body) {
        width: 100%;
        height: 100%;
    }
    .main-wrapper {
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: row;
    }
    .sidebar {
        background-color: blue;
        width: 200px;
        height: 100%;
    }
    .content {
        display: flex;
        flex-direction: column;
    }
</style>