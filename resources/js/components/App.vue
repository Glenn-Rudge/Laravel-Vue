<template>
    <div>
        <h1 class="text-center text-9xl text-cyan-500">{{ title }}</h1>

        <div class="py-7">
            <h3 class="text-3xl text-center">Counter: {{ count }}</h3>
            <div class="pt-5 text-center">
                <button
                    @click="increment"
                    class="py-2 px-5 bg-blue-700 mr-5 hover:bg-blue-500"
                >
                    Add
                </button>
                <button
                    @click="decrement"
                    class="p-2 px-5 bg-emerald-700 hover:bg-emerald-500"
                >
                    Decrement
                </button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            title: "VueJS 3 And Laravel",
            count: 0,
        };
    },

    methods: {
        increment() {
            return this.count++;
        },

        decrement() {
            return this.count--;
        },
    },
};
</script>

<style scoped></style>
