<script>
import Heading from "@/components/Heading/Heading.vue";

export default {
    name: "Links",
    components: {Heading},

    computed: {
        links() {
            return [
                {
                    href: 'https://t.me/elongsol',
                    url: '/img/links/tg.svg',
                    alt: 'telegram'
                },
                {
                    href: 'https://x.com/elongtomars?s=21',
                    url: '/img/links/twitter.svg',
                    alt: 'x'
                },
                {
                    href: 'https://coinmarketcap.com/',
                    url: '/img/links/cmc.svg',
                    alt: 'cmc'
                },
                {
                    href: 'https://dexscreener.com/solana/2on42hk6vxqeskwmdrvikkhacmu2h5rdiuszmwm4w1ks',
                    url: '/img/links/dex.svg',
                    alt: 'dexscreener'
                },
                {
                    href: 'https://www.coingecko.com/ru',
                    url: '/img/links/coingecko.svg',
                    alt: 'coingecko'
                },
            ]
        }
    }
}
</script>

<template>
    <div class="links">
        <Heading title="VISIT OUR LINKS " />
        <div class="container">
            <div class="links__content">
                <a v-for="(link, index) in links"
                   :href="link.href"
                   :key="index"
                   target="_blank"
                >
                    <img :src="link.url"
                         :alt="link.alt"
                         class="links__item--img"
                    />
                </a>
            </div>
        </div>
    </div>
</template>

<style src="./links.css" scoped/>