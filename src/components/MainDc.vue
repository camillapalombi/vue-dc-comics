<template>
    <div>
        <section class="section-main-top">
            <img src="../../src/assets/img/jumbotron.jpg" alt="ciao">
        </section>

        <section class="section-main-bottom">

            <div class="label-current-series">CURRENT SERIES</div>

            <div class="container container-box-series">
                <BoxSeries v-for="serie in currentSeries" :key="serie.series" :src-image="serie.thumb" :serie-title="serie.series"/>
            </div>

            <div class="container-btn-load">
                <div class="btn-load-more">LOAD MORE</div>
            </div>

        </section>
    </div>
</template>

<script>
import BoxSeries from '../components/BoxSeries.vue'

export default {
name: 'MainDc',
data () {
    return {
        currentSeries: [
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                            price: "$19.99",
                            series: "Action Comics",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                            price: "$3.99",
                            series: "American Vampire 1976",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                            price: "$16.99",
                            series: "Aquaman",
                            type: "graphic novel"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                            price: "$2.99",
                            series: "Batgirl",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                            price: "$3.99",
                            series: "Batman",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                            price: "$2.99",
                            series: "Batman Beyond",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                            price: "$3.99",
                            series: "Batman/Superman",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                            price: "$4.99",
                            series: "Batman/Superman Annual",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                            price: "$5.99",
                            series: "Batman: The Joker War Zone",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                            price: "$6.99",
                            series: "Batman: Three Jokers",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                            price: "$4.99",
                            series: "Batman: White Knight Presents: Harley Quinn",
                            type: "comic book"
                        },
                        {
                            thumb: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                            price: "$16.99",
                            series: "Catwoman",
                            type: "graphic novel"
                        }
                    ]
    }
            
        },
        components: {
            BoxSeries
        }
}
</script>

<style scoped lang="scss">
@import '../assets/style/partials/variables';

.section-main-top {
    width: 100%;
    height: 30rem;
    img {
        height: 100%;
        width: 100%;
    }
}
.section-main-bottom {
    width: 100%;
    height: 50rem;
    background-color: $contentBackground;
    position: relative;

    .container-box-series {
        display: flex;
        flex-wrap: wrap;
        justify-content: flex-start;
        align-items: stretch;
        padding-top: 70px;
    }
}

.label-current-series {
    width: 180px;
    padding: 1em;
    text-align: center;
    color: white;
    background-color: $activeColor;
    font-weight: bold;
    font-size: 15px;
    position: absolute;
    top: -20px;
    left: 200px;
}

.container-btn-load {
    display: flex;
    justify-content: center;
    margin-top: 30px;
        .btn-load-more {
        width: 150px;
        padding: 1em;
        text-align: center;
        color: white;
        background-color: $activeColor;
        font-weight: bold;
        cursor: pointer;
        }
}
</style>