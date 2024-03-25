<template>
    <section class="counter">
        <div class="counter-box">
            <div class="counter-box__item" v-for="counter in counters" :key="counter.id">
                <div class="counter-box__item-inner">
                    <h2 class="counter-box__item-title">{{ counter.title }}</h2>
                    <p class="counter-box__item-text">{{ counter.text }}</p>
                </div>
            </div>
            <!-- <div class="counter-box__item">
                <div class="counter-box__item-inner">
                    <h2 class="counter-box__item-title">12</h2>
                    <p class="counter-box__item-text">Years of Experience</p>
                </div>
            </div>
            <div class="counter-box__item">
                <div class="counter-box__item-inner">
                    <h2 class="counter-box__item-title">85</h2>
                    <p class="counter-box__item-text">Success Project</p>
                </div>
            </div>
            <div class="counter-box__item">
                <div class="counter-box__item-inner">
                    <h2 class="counter-box__item-title">15</h2>
                    <p class="counter-box__item-text">Active Project</p>
                </div>
            </div>
            <div class="counter-box__item">
                <div class="counter-box__item-inner">
                    <h2 class="counter-box__item-title">95</h2>
                    <p class="counter-box__item-text">Happy CUstomers</p>
                </div>
            </div> -->
        </div>
    </section>
</template>

<script>
export default {
    name: 'CounterComponent',

    data() {
        return {
            counters: [
                {
                    id: 1,
                    title: '12',
                    text: 'Years of Experience',
                },
                {
                    id: 2,
                    title: '85',
                    text: 'Success Project',
                },
                {
                    id: 3,
                    title: '15',
                    text: 'Active Project',
                },
                {
                    id: 4,
                    title: '95',
                    text: 'Happy CUstomers',
                }
            ]

        };
    },

    mounted() {

    },

    methods: {

    },
};
</script>