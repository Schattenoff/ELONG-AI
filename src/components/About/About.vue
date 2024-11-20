<script>

export default {
    name: "About",


    methods: {
        handleCopy() {
            navigator.clipboard.writeText('63P6eXUeGs43h9sLzfn3cBnHGTJNr7XSpvqokxoZpump')
                .then(() => {

                })
                .catch(() => {

                });
        }
    }
}
</script>

<template>
    <div class="about">
        <div class="container">
            <div class="about__content">
                <img class="about__img" src="/img/Elong.png" />
                <div class="about__btn" @click="handleCopy()">Contract Address</div>
                <div class="about__text">Powered by blockchain technology, ELONG AI offers a playful entry into the world of cryptocurrency, where Musk-inspired memes meet the thrill of market speculation.</div>
            </div>
        </div>
    </div>
</template>

<style src="./about.css" scoped/>