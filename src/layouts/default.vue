<template>
    <div>
        <MetaTags/>
        <div class="flex flex-col pg-surface pg-on-surface-text">
            <NavBar class="fixed pg-surface shadow z-10"/>
            <div class="mt-24 shadow">
                <router-view/>
            </div>
            <TheFooter/>
        </div>
    </div>
</template>
<style></style>
