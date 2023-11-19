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

        <div class="container px-4 px-lg-5">
            <div class="row gx-4 gx-lg-5 justify-content-center">
                <form>
                    <div class="mb-3">
                        <label for="title" class="form-label">Title</label>
                        <input
                            type="text"
                            class="form-control"
                            id="title"
                            aria-describedby="title"
                        />
                    </div>
                    <div class="mb-3">
                        <label for="body" class="form-label">Content</label>
                        <textarea
                            rows="8"
                            class="form-control"
                            placeholder="Leave a comment here"
                            id="body"
                        ></textarea>
                    </div>
                    <button type="submit" class="btn btn-primary mb-4">
                        Submit
                    </button>
                </form>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {};
    },
};
</script>
