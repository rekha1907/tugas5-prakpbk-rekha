<template>
  <q-card class="q-mb-md">
    <q-card-section>
      <div class="row">
        <div class="col-4" v-for="(product, index) in products" :key="index">
          <q-img :src="product.image" :alt="product.title" class="product-image"/>
          <div class="text-h6">{{ product.title }}</div>
          <div class="text-body2">{{ product.description }}</div>
          <q-btn label="Beli Sekarang" color="primary" class="q-mt-md" />
        </div>
      </div>
    </q-card-section>
  </q-card>
</template>

<script>
import bedakImage from '../assets/bedak.jpg';
import bojImage from '../assets/boj.webp';
import cushionImage from '../assets/cushion.png';
import facemaskImage from '../assets/facemask.jpg';
import micellarImage from '../assets/micellar.jpeg';
import moizImage from '../assets/moiz.jpg';
import serumImage from '../assets/serum.jpeg';
import sunscreenImage from '../assets/sunscreen.jpeg';
import tonerImage from '../assets/toner.jpg';

export default {
  data() {
    return {
      products: [
        { title: 'Bedak Padat', description: 'Wardah Colorfit Velvet Powder Foundation merupakan kombinasi foundation dan bedak yang terasa halus serta ideal untuk kulit kering', image: bedakImage },
        { title: 'Cleansing Oil', description: 'The Beauty of Joseon Ginseng Cleansing Oil adalah minyak pembersih lembut dan ringan sekaligus menambah kelembapan pada kulit.', image: bojImage },
        { title: 'Cushion', description: 'Cover All Perfect Cushion dapat membantu mengontrol minyak untuk mencegah kusam dan warna tidak merata serta mencerahkan kulit wajah.', image: cushionImage },
        { title: 'Facial Mask', description: 'Masker wajah anti penuaan yang meremajakan untuk kulit sempurna, mengurangi garis-garis halus & melembabkan kulit Anda.', image: facemaskImage },
        { title: 'Micellar', description: 'SKINTIFIC Mugwort Purifying Micellar Water merupakan micellar water dengan kandungan Mugwort, Centella, dan Ceramide, membersihkan wajah dari kotoran.', image: micellarImage },
        { title: 'Neutrogena', description: 'Neutrogena Hydro Boost Water Gel pelembab wajah, menyegarkan untuk membuat kulit bersinar. Ideal untuk kulit kering, sensitif, & berjerawat.', image: moizImage },
        { title: 'Serum', description: 'Kadar antioksidan di malam hari memperbaiki kerutan halus, mengencangkan kulit & meningkatkan kecerahan, efektif untuk semua jenis & warna kulit.', image: serumImage },
        { title: 'Sun Screen', description: 'Tabir surya dalam bentuk gel (water base) yang diformulasi khusus dengan tekstur yang ringan, nyaman, dan tanpa whitecast.', image: sunscreenImage },
        { title: 'Toner', description: 'Toner wajah membantu membersihkan wajah dari sisa kotoran, menyeimbangkan PH wajah, mencerahkan kulit wajah, merawat kulit berjerawat.', image: tonerImage },
      ]
    };
  }
};
</script>

<style scoped>
.product-image {
  width: 100%;
  height: auto;
  max-width: 200px;  /* Adjust the max-width as per your requirement */
  max-height: 200px; /* Adjust the max-height as per your requirement */
  display: block;
  margin-left: auto;
  margin-right: auto;
}
</style>
