<template>
  <main class="container">
    <section-product></section-product>
    <div class="flex flex-col w-full mt-24">
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl md:text-left mb-2 text-2xl text-center"
      >
        ISA-ERP
      </h1>
      <p
        class="md:pt-0 md:text-2xl lg:text-2xl md:mb-12 lg:text-left mt-4 mb-12 text-lg text-center"
      >
        ISA-ERP programski paket je skup međusobno povezanih programskih modula
        ili podprograma koji čine kompletni poslovno informacioni sistem.
      </p>
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl md:text-left mb-2 text-2xl text-center"
      >
        Moduli
      </h1>
      <!-- MODULE CONTAINER -->
      <div class="modules-container container my-12">
        <!-- 1st -->
        <div
          class="md:grid-cols-3 modules-grid grid grid-cols-1 gap-4 py-6 text-center bg-yellow-300 rounded-md"
        >
          <div>Finansijsko knjigovodstvo</div>
          <div>Robno knjigovodstvo - Veleprodaja</div>
          <div>Robno knjigovodstvo - Maloprodaja</div>
        </div>
        <!-- 2nd -->
        <div
          class="md:grid-cols-3 modules-grid grid grid-cols-1 gap-4 py-6 text-center bg-white rounded-md shadow-inner"
        >
          <div>POS Kasa</div>
          <div>Materijalno knjigovodstvo</div>
          <div>Proizvodnja na bazi normativa</div>
        </div>
        <!-- 3rd -->
        <div
          class="md:grid-cols-3 modules-grid grid grid-cols-1 gap-4 py-6 text-center bg-yellow-300 rounded-md"
        >
          <div>Fakturisanje usluga</div>
          <div>
            Knjiga ulaznih faktura, knjiga izlaznih faktura i generisanje PDV
            prijave
          </div>
          <div>Blagajna</div>
        </div>
        <!--  -->
        <!--  -->
        <!-- 1st -->
        <div
          class="md:grid-cols-3 modules-grid grid grid-cols-1 gap-4 py-6 text-center bg-white rounded-md"
        >
          <div>Plate</div>
          <div>Kadrovska evidencija</div>
          <div>Stalna sredstva</div>
        </div>
        <!-- 2nd -->
        <div
          class="md:grid-cols-3 modules-grid grid grid-cols-1 gap-4 py-6 text-center bg-yellow-300 rounded-md shadow-inner"
        >
          <div>Putni nalozi</div>
          <div>Virmani</div>
          <div>Finansijske knjižne obavijesti</div>
        </div>
      </div>
      <p
        class="md:pt-0 md:text-xl lg:text-xl md:mb-12 lg:text-left mt-4 mb-12 text-lg text-center"
      >
        ISA-ERP je u potpunosti usklađen s pozitivnim zakonskim propisima u
        Federaciji Bosne i Hercegovine i Republici Srpskoj. Na sve eventualne
        izmjene i dopune zakonskih propisa se reaguje u najkraćem mogućem roku i
        programi se odmah usklađuju s eventualnim izmjenama.
      </p>
      <!-- CARDS/MODULES -->
      <h1
        class="shippori md:pt-10 md:text-3xl lg:text-4xl md:text-left mb-2 text-2xl text-center"
      >
        Opšte Karakteristike
      </h1>
      <!--  -->
      <!--  -->
      <!-- 1st row -->
      <div
        class="md:flex-row md:space-x-24 md:space-y-0 container flex flex-col justify-center mt-12 space-y-8"
      >
        <service-card
          id="a"
          class="mx-auto"
          title="All-In-One Sistem"
          desc="Svi moduli i svi elementi se nalaze u jednom programu i međusobno su povezani. Podaci uneseni u jednom modulu su odmah i u drugom modulu na raspolaganju, tako da nema duplog unosa podataka."
          img-url="/images/product/characteristics/domain.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Jednostavnost Korištenja"
          desc="Korisnički interfejs (GUI) osmišljen je da omogući korisniku da na jednostavan način evidentira, obradi i izvjesti o svim poslovnim promjenama."
          img-url="/images/product/characteristics/popular.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Centralizovana Baza Podataka"
          desc="Svi korisnici sistema pristupaju jednoj bazi podataka čime se smanjuje mogućnost duplikacije podataka, netačnih podataka ili neusklađenosti podataka."
          img-url="/images/product/characteristics/server.svg"
        ></service-card>
      </div>
      <!--  -->
      <!--  -->
      <!-- 2nd row -->
      <div
        class="md:flex-row md:space-x-24 md:space-y-0 container flex flex-col justify-center mt-12 space-y-8"
      >
        <service-card
          id="a"
          class="mx-auto"
          title="Automatska Zaštita Podataka"
          desc="Za sigurnost, integritet i arhiviranje podataka brine se sistem za upravljanje bazama podataka. Vaši podaci su uvijek sigurni i na mjestu."
          img-url="/images/product/characteristics/shield.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Nadogradnja Programa"
          desc="Praćenjem globalnih tehnoloških trendova u mogućnosti smo da u vrlo kratkom vremenskom roku i bez ograničenja mijenjamo i nadograđujemo postojeći informacioni sistem."
          img-url="/images/product/characteristics/rocket.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Korisnička Prava"
          desc="U zavisnosti od pozicije u preduzeću, svakom korisniku je moguće dodijeliti određen nivo ovlaštenja i pristupa programu i podataka koje može vidjeti/mijenjati."
          img-url="/images/product/characteristics/girl.svg"
        ></service-card>
      </div>
      <!--  -->
      <!--  -->
      <!-- 3rd row -->
      <div
        class="md:flex-row md:space-x-24 md:space-y-0 container flex flex-col justify-center mt-12 space-y-8"
      >
        <service-card
          id="a"
          class="mx-auto"
          title="Elektronsko Poslovanje"
          desc="Omogućena je komunikacija sa programima svih banaka radi jednostavnijeg importa platnih naloga u program banke."
          img-url="/images/product/characteristics/laptop.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Uvoz - Izvoz Podataka"
          desc="Mogućnost uvoza podataka iz različitih formata: Txt, Excel, XML, DBF i ostale. Slanje dokumenata putem e-pošte direktno iz programa, izvoz dokumenata u Word, Excel, HTML, XML, PDF i druge formate dokumenata."
          img-url="/images/product/characteristics/import-export.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Mobilna Aplikacija"
          desc="ISA-ERP je u potpunosti prilagođen vašem mobilnom uređaju tako da možete u svakom momentu, na svakoj lokaciji da pristupite vašim podacima. U svakom momentu imate pristup bazi podataka."
          img-url="/images/product/characteristics/chat-bubble.svg"
        ></service-card>
      </div>
      <!--  -->
      <!--  -->
      <!-- 4th row -->
      <div
        class="md:flex-row md:space-x-24 md:space-y-0 container flex flex-col justify-center mt-12 mb-12 space-y-8"
      >
        <service-card
          id="a"
          class="mx-auto"
          title="Rad u mreži, lokalna i udaljena"
          desc="Neograničen broj istovremenih korisnika koji pristupaju istoj bazi podataka iz bilo kog modula."
          img-url="/images/product/characteristics/framework.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Fiskalizacija i izvještaji"
          desc="ISA-ERP radi sa svim fiskalnim uređajima koji su prisutni na tržištu BiH. ISA-ERP nudi više od 300 različitih izvještaja po raznim kriterijima uz kontinuirano kreiranje novih u zavisnosti od potreba, ideja i zahtjeva."
          img-url="/images/product/characteristics/fiscal.svg"
        ></service-card>
        <div class="md:w-70 md:block hidden"></div>
        <service-card
          id="a"
          class="mx-auto"
          title="Knjigovodstvo"
          desc="Potpuna integracija pomoćnih knjigovodstava sa glavnom knjigom (Podatak unesen na jednom mjestu koriste svi programski moduli). ISA-ERP radi sa svim fiskalnim uređajima koji su prisutni na tržištu BiH."
          img-url="/images/product/characteristics/book.svg"
        ></service-card>
      </div>
    </div>
  </main>
</template>

<script>
import SectionProduct from '@/components/sections/SectionProduct.vue'
import ServiceCard from '@/components/cards/SimpleCard.vue'

export default {
  name: 'ProductPage',
  components: {
    SectionProduct,
    ServiceCard,
  },
}
</script>

<style scoped>
@media only screen and (max-width: 1024px) {
  #footer-image {
    max-width: 350px;
    height: auto;
    margin: auto;
  }
}
</style>
