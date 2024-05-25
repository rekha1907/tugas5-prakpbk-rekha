<template>
  <q-card class="q-mb-md">
    <q-card-section>
      <div class="row">
        <div class="col-4" v-for="(product, index) in products" :key="index">
          <q-img :src="`./src/assets/${product.image}`" :alt="product.title" class="product-image"/>
          <div class="text-h6">{{ product.title }}</div>
          <div class="text-body2">{{ product.description }}</div>
          <q-btn label="Beli Sekarang" color="primary" class="q-mt-md" />
        </div>
      </div>
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  data() {
    return {
      products: [
        { title: 'Bedak Padat', description: 'Wardah Colorfit Velvet Powder Foundation merupakan kombinasi foundation dan bedak yang terasa halus. serta Ideal untuk kulit kering', image: '/src/assest/bedak.jpg' },
        { title: 'Cleansing Oil', description: 'The Beauty of Joseon Ginseng Cleansing Oil adalah minyak pembersih lembut dan ringan sekaligus menambah kelembapan pada kulit.', image: '/src/assets/boj.webp' },
        { title: 'Cushion', description: 'Cover All Perfect Cushion Dapat membantu mengontrol minyak untuk mencegah kusam dan warna tidak merata serta mencerahkan kulit wajah.', image: '/src/assets/cushion.png' },
        { title: 'Facial Mask', description: 'Masker Wajah Anti Penuaan yang Meremajakan Untuk Kulit Sempurna-Mengurangi Garis-garis Halus & Melembabkan Kulit Anda.', image: '/src/assets/facemask.jpg' },
        { title: 'Micellar', description: 'SKINTIFIC Mugwort Purifying Micellar Water merupakan micellar water dengan kandungan Mugwort, Centella, dan Ceramide, membersihkan wajah dari kotoran.', image: '/src/assets/micellar.jpeg' },
        { title: 'Neutrogena', description: 'Neutrogena Hydro Boost Water Gel Pelembab Wajah, menyegarkan untuk membuat kulit bersinar. Ideal untuk kulit kering, sensitif, & berjerawat.', image: '/src/assets/moiz.jpg' },
        { title: 'Serum', description: 'Kadar antioksidan di malam hari memperbaiki kerutan halus, mengencangkan kulit & meningkatkan kecerahan, Efektif untuk semua jenis & warna kulit.', image: '/src/assets/serum.jpeg' },
        { title: 'Sun Screen', description: ' tabir surya dalam bentuk gel (water base) yang diformulasi khusus dengan tekstur yang ringan, nyaman, dan tanpa whitecast.', image: '/src/assets/sunscreen.jpeg' },
        { title: 'Toner', description: 'Toner wajah membantu membersihkan wajah dari sisa kotoran, menyeimbangkan PH wajah, mencerahkan kulit wajah, merawat kulit berjerawat.', image: '/src/assets/toner.jpg' },
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
