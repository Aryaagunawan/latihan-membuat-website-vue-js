<template>
    <div>
        <header
            class="masthead"
            style="background-image: url('/img/post-sample-image.jpg')"
        >
            <div class="container position-relative px-4 px-lg-5">
                <div class="row gx-4 gx-lg-5 justify-content-center">
                    <div class="col-md-10 col-lg-8 col-xl-7">
                        <div class="site-heading">
                            <h1>@duniacoding Vue Blog</h1>
                            <span class="subheading"
                                >A Blog Theme by Dunia Coding</span
                            >
                        </div>
                    </div>
                </div>
            </div>
        </header>

        <!-- Post -->
        <div class="container px-4 px-lg-5">
            <div class="row gx-4 gx-lg-5 justify-content-center">
                <div class="col-md-10 col-lg-8 col-xl-7">
                    <div class="d-flex justify-content-end mb-4">
                        <RouterLink
                            to="/blogs/add"
                            class="btn btn-primary text-uppercase"
                            >Add Blog</RouterLink
                        >
                    </div>
                    <div
                        v-for="(data, index) of blogs"
                        :key="'index-blogs-' + index"
                    >
                        <div class="post-preview">
                            <RouterLink :to="'/blogs/' + data.id">
                                <h2 class="post-title">
                                    {{ data.title }}
                                </h2>
                                <h3 class="post-subtitle">
                                    {{ data.body.slice(0, 80) }}
                                </h3>
                            </RouterLink>
                            <p class="post-meta">
                                Posted by
                                <a href="#!">Alfian Luthfi</a>
                                on September 24, 2022
                            </p>
                        </div>
                        <hr class="my-4" />
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            blogs: [
                {
                    id: 1,
                    title: "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
                    body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus eveniet illum ullam reprehenderit repellat eius iusto? Vel ipsam velit, cumque totam nulla, tenetur aliquid dolore rem molestiae repellat, autem ullam nemo debitis sit dignissimos reprehenderit officia? Ipsum quam deleniti odio.",
                },
                {
                    id: 2,
                    title: "qui est esse",
                    body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus eveniet illum ullam reprehenderit repellat eius iusto? Vel ipsam velit, cumque totam nulla, tenetur aliquid dolore rem molestiae repellat, autem ullam nemo debitis sit dignissimos reprehenderit officia? Ipsum quam deleniti odio. Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus eveniet illum ullam reprehenderit repellat eius iusto? Vel ipsam velit, cumque totam nulla, tenetur aliquid dolore rem molestiae repellat, autem ullam nemo debitis sit dignissimos reprehenderit officia? Ipsum quam deleniti odio.",
                },
                {
                    id: 3,
                    title: "ea molestias quasi exercitationem repellat qui ipsa sit aut",
                    body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus eveniet illum ullam reprehenderit repellat eius iusto? Vel ipsam velit, cumque totam nulla, tenetur aliquid dolore rem molestiae repellat, autem ullam nemo debitis sit dignissimos reprehenderit officia? Ipsum quam deleniti odio.",
                },
                {
                    id: 4,
                    title: "eum et est occaecati",
                    body: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus eveniet illum ullam reprehenderit repellat eius iusto? Vel ipsam velit, cumque totam nulla, tenetur aliquid dolore rem molestiae repellat, autem ullam nemo debitis sit dignissimos reprehenderit officia? Ipsum quam deleniti odio. Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus eveniet illum ullam reprehenderit repellat eius iusto? Vel ipsam velit, cumque totam nulla, tenetur aliquid dolore rem molestiae repellat, autem ullam nemo debitis sit dignissimos reprehenderit officia? Ipsum quam deleniti odio. Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus eveniet illum ullam reprehenderit repellat eius iusto? Vel ipsam velit, cumque totam nulla, tenetur aliquid dolore rem molestiae repellat, autem ullam nemo debitis sit dignissimos reprehenderit officia? Ipsum quam deleniti odio.",
                },
            ],
        };
    },
};
</script>
