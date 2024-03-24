<script setup>
defineProps({
    msg: {
        type: String,
        required: true,
    },
});
</script>

<template>
    <div class="greetings">
        <h1 class="green">{{ msg }}</h1>
        <h3>
            You’ve successfully created a project with
            <a href="https://vitejs.dev/" target="_blank" rel="noopener"
                >Vite</a
            >
            +
            <a href="https://vuejs.org/" target="_blank" rel="noopener">Vue 3</a
            >.
            <p class="name">
                <input type="text" placeholder="Enter your name" />
                <a href="">asadas</a>
            </p>
        </h3>
    </div>
</template>

<style scoped lang="scss">
h1 {
    font-weight: 500;
    font-size: 2.6rem;
    position: relative;
    top: -10px;
}

h3 {
    font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
    text-align: center;
}

@media (min-width: 1024px) {
    .greetings h1,
    .greetings h3 {
        text-align: left;
    }
}
.name {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
    input {
        padding: 5px;
        border: 1px solid #b95842;
        border-radius: 5px;
    }
    a {
        color: #b95842;
    }
}
</style>
