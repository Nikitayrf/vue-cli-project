<template>
    <section class="blog">
        <div class="latest-post">
            <h2 class="latest-post__heading">Latest Post</h2>
            <div class="latest-post__box">
                <img class="latest-post__img" :src="require('@/assets/img/kitche_with_marble_island.png')"
                    alt="latest post" />
                <div class="latest-post__content-box">
                    <div class="latest-post__content">
                        <h3 class="latest-post__title">
                            Low Cost Latest Invented Interior Designing Ideas
                        </h3>
                        <p class="latest-post__text">
                            Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae
                            turpis dignissim maximus.posuere in.Contrary to popular
                            belief.
                            <br />
                            Lorem Ipsum is not simply random text. It has roots in a piece
                            of classica.
                        </p>
                    </div>
                    <div class="latest-post-nav">
                        <span class="article-nav__date-news">26 December,2022 </span>
                        <svg class="latest-post-nav__arrow" width="70" height="70" viewBox="0 0 70 70" fill="none"
                            xmlns="http://www.w3.org/2000/svg">
                            <circle cx="35" cy="35" r="35" fill="#F4F0EC" />
                            <path d="M32 44L40 35L32 26" stroke="#292F36" stroke-width="2" stroke-linecap="round"
                                stroke-linejoin="round" />
                        </svg>
                    </div>
                </div>
            </div>
        </div>

        <div class="news-articles">
            <h2 class="news-articles__title">Articles & News</h2>
            <div id="app" class="news-box">
                <article class="news" v-for="news in listNews.slice(0, 6)" :key="news.id">
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

        <div class="pagination">
            <div class="pagination-box">
                <div class="pagination__item pagination__item-active">
                    <div class="pagination__text">01</div>
                </div>
                <div class="pagination__item">
                    <div class="pagination__text">02</div>
                </div>
                <div class="pagination__item">
                    <div class="pagination__text">03</div>
                </div>
                <div class="pagination__item">
                    <div class="pagination__text">></div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'BlogBigComponent',

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
                    image: require('@/assets/img/kitchen_sink_hood.png'),
                    title: "Best For Any Office & Business Interior Solution",
                    date: "25 December,2022",
                },
                {
                    id: 4,
                    tag: "Kitchan Design",
                    image: require('@/assets/img/kitchen_beige_four_lamp.png'),
                    title: "Let’s Get Solution For Building Construction Work",
                    date: "26 December,2022",
                },
                {
                    id: 5,
                    tag: "Living Design",
                    image: require('@/assets/img/room_with_two_chair_one_sofa.png'),
                    title: "Low Cost Latest Invented Interior Designing Ideas.",
                    date: "22 December,2022",
                },
                {
                    id: 6,
                    tag: "Interior Design",
                    image: require('@/assets/img/kitchen_four_chez.png'),
                    title: "Best For Any Office & Business Interior Solution",
                    date: "25 December,2022",
                },
                {
                    id: 7,
                    tag: "Kitchan Design",
                    image: require('@/assets/img/kitche_with_marble_island.png'),
                    title: "Low Cost Latest Invented Interior Designing Ideas",
                    text: "Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpis dignissim maximus.posuere in.Contrary to popular belief. Lorem Ipsum is not simply random text. It has roots in a piece of classica.",
                    date: "26 December,2022",
                },
            ],
        };
    },
};
</script>