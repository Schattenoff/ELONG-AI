<script>
import Header from "@/components/Header/Header.vue";
import ContractAddress from "@/components/ContractAddress/ContractAddress.vue";
import About from "@/components/About/About.vue";
import Mint from "@/components/Mint/Mint.vue";
import Links from "@/components/Links/Links.vue";

export default {
    name: "App",
    components: {
        Links,
        Mint,
        About,
        ContractAddress,
        Header
    }
}
</script>

<template>
    <Header />
    <ContractAddress />
    <About />
    <Mint />
    <Links />
</template>

<style src="./app.css" />