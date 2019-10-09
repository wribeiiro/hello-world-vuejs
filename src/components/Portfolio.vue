<template>
    <section class="bg-light" id="portfolio">
      <div class="container">
        <div class="row">
          <div class="col-lg-12 text-center">
            <h2 class="section-heading text-uppercase">Portfolio</h2>
            <h3 class="section-subheading text-muted">Lorem ipsum dolor sit amet consectetur.</h3>
          </div>
        </div>
        <div class="row">
          
            <div class="col-md-4 col-sm-6 portfolio-item" v-for="(obj, key) in arrayPortfolio" :key="key">
                <a class="portfolio-link" data-toggle="modal" href="#portfolioModal2">
                    <div class="portfolio-hover">
                        <div class="portfolio-hover-content">
                            <i class="fas fa-plus fa-3x"></i>
                        </div>
                    </div>
                    <img class="img-fluid" src="img/header-bg.jpg" alt="">
                </a>
                <div class="portfolio-caption">
                    <h4>{{ obj.legend }}</h4>
                    <p class="text-muted">{{ obj.title }}</p>
                </div>
            </div>
        </div>
      </div>
    </section>
</template>

<script>
export default {
    data: () => ({
        arrayPortfolio: [
            {
                img: 'img/header-bg.jpg',
                legend: 'Finish',
                title: 'Finish Him'
            },
            {
                img: 'img/header-bg.jpg',
                legend: 'Lines',
                title: 'Lines'
            },
            {
                img: 'img/header-bg.jpg',
                legend: 'Southwest',
                title: 'Website'
            },
            {
                img: 'img/header-bg.jpg',
                legend: 'Window',
                title: 'XP'
            },
            {
                img: 'img/header-bg.jpg',
                legend: 'Coffee',
                title: 'Break!' 
            },
            {
                img: 'img/header-bg.jpg',
                legend: 'Dashboard',
                title: 'hum D;!'
            }
        ]
    })
}
</script>

<style lang="css">

</style>


