<template>
    <section class="blog">
        <div class="blog__heading">
            <h2 class="blog__heading-title">Articles & News</h2>
            <p class="blog__heading-text">
                It is a long established fact that a reader will be distracted by
                the of readable content of a page when lookings at its layouts the
                points of using.
            </p>
        </div>
        <div class="news-articles">
            <div id="app" class="news-box">
                <article class="news" v-for="news in listNews.slice(0, 3)" :key="news.id">
                    <div class="news__content">
                        <img class="news__img" :src="news.image" alt="" />
                        <a class="news__button" href="#">Kitchan Design</a>
                        <h3 class="news__title">{{ news.title }}</h3>

                        <div class="news-nav">
                            <span class="news-nav__date-news">{{ news.date }}</span>
                            <svg class="news-nav__arrow" width="70" height="70" viewBox="0 0 70 70" fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <circle cx="35" cy="35" r="35" fill="#F4F0EC" />
                                <path d="M32 44L40 35L32 26" stroke="#292F36" stroke-width="2" stroke-linecap="round"
                                    stroke-linejoin="round" />
                            </svg>
                        </div>
                    </div>
                </article>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'BlogComponent',

    data() {
        return {
            listNews: [
                {
                    id: 1,
                    tag: "Kitchan Design",
                    image: require('@/assets/img/kitchen_four_chez.png'),
                    title: "Let’s Get Solution For Building Construction Work",
                    date: "26 December,2022",
                },
                {
                    id: 2,
                    tag: "Living Design",
                    image: require('@/assets/img/kitchen_with_view_door.png'),
                    title: "Low Cost Latest Invented Interior Designing Ideas.",
                    date: "22 December,2022",
                },
                {
                    id: 3,
                    tag: "Interior Design",
                    image: require('@/assets/img//kitchen_sink_hood.png'),
                    title: "Best For Any Office & Business Interior Solution",
                    date: "25 December,2022",
                },
            ],
        };
    },

};
</script>