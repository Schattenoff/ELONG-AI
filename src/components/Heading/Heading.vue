<script>
export default {
    name: "Heading",

    props: {
        title: String,
    }
}
</script>

<template>
    <div class="heading">
        <div class="container">
            <h2 class="heading__title">
                {{title}}
            </h2>
        </div>
    </div>
</template>

<style src="./heading.css" scoped/>