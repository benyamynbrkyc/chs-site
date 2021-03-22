<template>
  <main>
    <section-hero class="mt-8"></section-hero>

    <div class="flex flex-col w-full mt-24">
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl mb-8 text-2xl text-center"
      >
        Usluge
      </h1>
    </div>

    <section class="flex-col mt-24 mb-24 space-y-32">
      <section-services class=""></section-services>
    </section>

    <div class="flex flex-col w-full mt-24">
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl mb-8 text-2xl text-center"
      >
        Vodeći Računovodstveni Software
      </h1>
    </div>

    <section class="container flex-col mt-24 mb-24 space-y-32">
      <section-featured-ltr
        small-title="ENTERPRISE RESOURCE PLANNING"
        main-title="Najbolji All-In-One racunovodstveni sistem"
        desc="Testiran na bazama podataka gdje je veličina jedne datoteke preko 1.000.000.000 zapisa, ISA-ERP je odlična solucija za sve biznise - velike i male."
        button-link="/"
        button-text="Saznajte Više"
        img-url="/images/product/ISA-ERP.png"
        class="flex"
      ></section-featured-ltr>

      <p
        class="md:pt-0 md:text-xl lg:text-xl md:mb-12 lg:text-left block max-w-xl mx-auto mt-4 mb-12 text-lg text-center"
      >
        Svi moduli i svi elementi se nalaze u jednom programu i međusobno su
        povezani. Podaci uneseni u jednom modulu su odmah i u drugom modulu na
        raspolaganju, tako da nema duplog unosa podataka.
      </p>

      <section-featured-rtl
        small-title="PRISTUPAČNOST"
        main-title="Ne želite komplikovane procedure tipkanja i tabele? Ni mi."
        desc="Sa ISA-ERP softverskim paketom korisničko iskustvo stavljamo na prvo mjesto. Računovodstvo ne mora biti dosadno."
        button-link="/"
        button-text="Saznajte Više"
        img-url="/images/home-featured/happy-people.png"
        class="flex"
      ></section-featured-rtl>

      <section-featured-ltr
        small-title="MOBILNA APLIKACIJA"
        main-title="Kompletna kontrola s vašeg pametnog uređaja."
        desc="ISA-ERP je u potpunosti prilagođen vašem mobilnom uređaju tako da možete da pristupite vašim podacima u svakom momentu, na svakoj lokaciji."
        button-link="/"
        button-text="Saznajte Više"
        img-url="/images/home-featured/isaerp-mobile.png"
        class="flex"
      ></section-featured-ltr>

      <section-featured-rtl
        small-title="SIGURNOST"
        main-title="Automatska enkripcija za maksimalnu sigurnost."
        desc="Za sigurnost, integritet i arhiviranje podataka brine se sistem za upravljanje bazama podataka. Razvijen sa posebnim akcentom na sigurnost, tako da manje brinete o podacima, a vise o rezultatima."
        button-link="/"
        img-url="/images/home-featured/cyber-security.png"
        class="flex"
      ></section-featured-rtl>

      <section-featured-ltr
        small-title="ELEKTRONSKO POSLOVANJE"
        main-title="Potpuna integracija sa programima banaka."
        desc="ISA-ERP čini elektronsko poslovanje lakšim nego ikada. Potpuno sinhronizovana komunikacija sa programima svih banaka, import platnih naloga, te export u Word, Excel, PDF i druge formate."
        button-link="/"
        img-url="/images/home-featured/payment.png"
        class="flex"
      ></section-featured-ltr>

      <section-featured-rtl
        small-title="MREŽA"
        main-title="Rad u mreži - lokalna i udaljena."
        desc="Neograničen broj istovremenih korisnika koji pristupaju istoj bazi podataka iz bilo kog modula. Potpuna integracija pomoćnih knjigovodstava sa glavnom knjigom (Podatak unesen na jednom mjestu koriste svi programski moduli)."
        button-link="/"
        img-url="/images/home-featured/network.png"
        class="flex"
      ></section-featured-rtl>
    </section>
  </main>
</template>

<script>
import SectionHero from '@/components/sections/SectionHero.vue'
import SectionFeaturedLtr from '@/components/sections/SectionFeaturedLtr.vue'
import SectionFeaturedRtl from '@/components/sections/SectionFeaturedRtl.vue'
import SectionServices from '@/components/sections/SectionServices.vue'

export default {
  name: 'IndexPage',
  components: {
    SectionHero,
    SectionFeaturedLtr,
    SectionFeaturedRtl,
    SectionServices,
  },
}
</script>
