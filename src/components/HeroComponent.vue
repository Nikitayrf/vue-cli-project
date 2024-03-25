<template>
    <section class="hero">
        <div class="hero__inner">
            <div class="hero__images">
                <img class="hero__images-item" :src="require('@/assets/img/hero.jpg')" alt="hero" />
            </div>

            <div class="hero__intro">
                <main class="hero__main">
                    <h1 class="hero__intro-title">Let Your Home Be Unique</h1>
                    <p class="hero__intro-text">
                        There are many variations of the passages of Lorem Ipsum
                        available, majority.
                    </p>
                </main>
                <button class="hero__btn">
                    <a href="#" class="hero__btn-link"></a>
                    Get Started
                    <svg class="hero__btn-icon" width="18" height="17" viewBox="0 0 18 17" fill="none"
                        xmlns="http://www.w3.org/2000/svg">
                        <path d="M1 8.43542L14.7232 8.29857M9.61818 1.91138L16.1412 8.43436L9.48677 15.0887"
                            stroke="#CDA274" stroke-width="2" stroke-linecap="square" stroke-linejoin="round" />
                    </svg>
                </button>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'HeroComponent',

};
</script>