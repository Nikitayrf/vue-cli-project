<template>
    <section class="project">
        <div class="project__heading">
            <h2 class="project__heading-title">Follow Our Projects</h2>
            <p class="project__heading-text">
                It is a long established fact that a reader will be distracted by
                the of readable content of page lookings at its layouts points.
            </p>
        </div>
        <ul class="project-box">
            <li class="project-box__item" v-for="project in projects" :key="project.id">
                <img class="project-box__img" :src="project.img" :alt="project.alt" />
                <div class="project-box__content">
                    <div class="project-box__info">
                        <h3 class="project-box__title">{{ project.title }}</h3>
                        <nav class="breadcrumbs">
                            <ul class="breadcrumbs__ul">
                                <li class="breadcrumbs__li">
                                    <a href="#" class="breadcrumbs__link">Decor</a>
                                </li>
                                <li class="breadcrumbs__li">
                                    <a href="#" class="breadcrumbs__link">Artchitecture</a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                    <svg class="product__arrow" width="70" height="70" viewBox="0 0 70 70" fill="none"
                        xmlns="http://www.w3.org/2000/svg">
                        <circle cx="35" cy="35" r="35" fill="#F4F0EC" />
                        <path d="M32 44L40 35L32 26" stroke="#292F36" stroke-width="2" stroke-linecap="round"
                            stroke-linejoin="round" />
                    </svg>
                </div>
            </li>

        </ul>
    </section>
</template>

<script>
export default {
    name: 'ProjectComponent',

    data() {
        return {
            projects: [
                {
                    id: 1,
                    title: 'Modern Kitchan',
                    img: require('@/assets/img/kitchen_with_microwave.jpg'),
                    alt: 'kitchen_with_microwave.jpg',
                },
                {
                    id: 2,
                    title: 'Modern Kitchan',
                    img: require('@/assets/img/chest_of_drawers_witch_two_mirrors.png'),
                    alt: 'chest_of_drawers_witch_two_mirrors.png',
                },
                {
                    id: 3,
                    title: 'Modern Kitchan',
                    img: require('@/assets/img/workspace_with_chez_and_white_lamp.png'),
                    alt: 'workspace_with_chez_and_white_lamp.png',
                },
                {
                    id: 4,
                    title: 'Modern Kitchan',
                    img: require('@/assets/img/room_with_four_chairs_and_four_pictures.png'),
                    alt: 'room_with_four_chairs_and_four_pictures.png',
                }
            ],

        };
    },

    mounted() {

    },

    methods: {

    },
};
</script>