<template>
  <div v-on:scroll="handleScroll">
      <Header :topOfPage="this.view.topOfPage"/>
      <div class="mx-20 my-10">
        <section>
          <h1 class="text-2xl font-bold" @click="checkScroll">Explorer Airbnb</h1>
          <div class="flex flex-row items-center">
            <div v-for="item in five" :key="item.id">
                <Five-Card :data=item />
            </div>
          </div>
        </section>
        <section>
          <div class="">
                <div v-for="item in six" :key="item.id">
                    <SixCard :data=item />
                </div>
          </div>
        </section>
        <section>
            <h1 class="text-2xl font-bold">Découvrez les aventures Airbnb</h1>
            <h5 class="mt-2 text-base text-gray-500 font-light w-5/12">
                Voyages de plusieurs jours organisés par des experts locaux avec
                activités, repas et logements compris
            </h5>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-4 mt-6">
                <div v-for="item in firsts" :key="item.id">
                    <FirstCard :data=item />
                </div>
            </div>
        </section>
    
        <section class="mt-20">
            <h1 class="text-2xl font-bold">Logements dans le monde entier</h1>
            <h5 class="mt-2 text-base text-gray-500 font-light w-5/12">
                Voyages de plusieurs jours organisés par des experts locaux avec
                activités, repas et logements compris
            </h5>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-x-4 gap-y-8 mt-6">
                <div v-for="item in seconds" :key="item.id">
                    <SecondCard :data=item />
                </div>
            </div>
        </section>
    
        <section class="mt-20">
            <h1 class="text-2xl font-bold">Expériences très bien notées</h1>
            <h5 class="mt-2 text-base text-gray-500 font-light w-5/12">
                Voyages de plusieurs jours organisés par des experts locaux avec
                activités, repas et logements compris
            </h5>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-4 mt-6">
                <div v-for="item in thirds" :key="item.id">
                    <FirstCard :data=item />
                </div>
            </div>
        </section>
    
        <section class="mt-20">
            <h1 class="text-2xl font-bold">Destinations Airbnb Plus à la Une</h1>
            <h5 class="mt-2 text-base text-gray-500 font-light w-5/12">
                Voyages de plusieurs jours organisés par des experts locaux avec
                activités, repas et logements compris
            </h5>
            <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-3 gap-4 mt-6">
                <div v-for="item in fourths" :key="item.id">
                    <ThirdCard :data=item />
                </div>
            </div>
        </section>
      </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      view: {
        topOfPage: true,
      },
      firsts: [
        {
          id: 1,
          location: 'Cayman Islands',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img1.png'
        },
        {
          id: 2,
          location: 'Uruguay',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img2.png'
        },
        {
          id: 3,
          location: 'Iceland',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img3.png'
        },
        {
          id: 4,
          location: 'Mongolia',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img4.png'
        },
        {
          id: 5,
          location: 'Bahrain',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img5.png'
        },
        {
          id: 6,
          location: 'Bosnia and Herzegovina',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img6.png'
        },
      ],
      seconds: [
        {
          id: 1,
          location: 'Toledo',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - Rp 800.000 / malam',
          rate: '4,98',
          img: '/img7.png'
        },
        {
          id: 2,
          location: 'Mesa',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '4,98',
          img: '/img8.png'
        },
        {
          id: 3,
          location: 'Utica',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '4,98',
          img: '/img9.png'
        },
        {
          id: 4,
          location: 'South Bend',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '4,98',
          img: '/img10.png'
        },
        {
          id: 5,
          location: 'Toledo',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '4,98',
          img: '/img11.png'
        },
        {
          id: 6,
          location: 'Mesa',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '4,98',
          img: '/img12.png'
        },
        {
          id: 7,
          location: 'Utica',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '4,98',
          img: '/img13.png'
        },
        {
          id: 8,
          location: 'South Bend',
          name: 'Superhost',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '4,98',
          img: '/img14.png'
        },
      ],
      thirds: [
        {
          id: 1,
          location: 'Cayman Islands',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img15.png'
        },
        {
          id: 2,
          location: 'Uruguay',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img16.png'
        },
        {
          id: 3,
          location: 'Iceland',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img17.png'
        },
        {
          id: 4,
          location: 'Mongolia',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img18.png'
        },
        {
          id: 5,
          location: 'Bahrain',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img19.png'
        },
        {
          id: 6,
          location: 'Bosnia and Herzegovina',
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          rate: '5.0',
          img: '/img20.png'
        },
      ],
      fourths: [
        {
          id: 1,
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          img: '/img21.png'
        },
        {
          id: 2,
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          img: '/img22.png'
        },
        {
          id: 3,
          name: '2 Nights PACKAGE All Inclusive',
          desc: 'À partir de 577€/personne - 3 jours',
          img: '/img23.png'
        },
      ],
      five: [
        {
          id: 1,
          name: 'Logements',
          img : '/img24.png'
        },
        {
          id: 2,
          name: 'Expériences',
          img: '/img25.png',
        },
        {
          id: 3,
          name: 'Aventures',
          img: '/img26.png'
        }
      ],
      six:[
        {
          id: 1,
          name: 'Hébergements Airbnb Plus',
          detail: 'Une sélection de logements vérifiés selon des critères de qualité et de design',
          img: '/img27.png',
          logo: ''
        }
      ]
    }
  },
  beforeMount() {
    window.addEventListener('scroll', this.handleScroll)
  },
  methods: {
    handleScroll(){
      if(window.pageYOffset>150){
        if(this.view.topOfPage) this.view.topOfPage = false
      } else {
        if(!this.view.topOfPage) this.view.topOfPage = true
      }
    }
  },
  mounted() {
  },
}
</script>