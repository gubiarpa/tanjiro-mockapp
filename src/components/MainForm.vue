<template>
  <div class="mx-5 mt-4">
    <h2 class="mb-5">
      Lista de Órdenes de Trabajo
    </h2>
    <v-data-table
      :headers="headers"
      :items="desserts"
      :items-per-page="10"
      class="elevation-1"
    ></v-data-table>
  </div>
</template>

<script>
export default {
  data () {
    return {
      headers: [
        {
          text: 'Cliente',
          align: 'start',
          sortable: false,
          value: 'name',
        },
        { text: 'OT', value: 'codOT' },
        { text: 'OT - Descripción', value: 'descOT' },
        { text: 'Carbs (g)', value: 'carbs' },
        { text: 'Protein (g)', value: 'protein' },
        { text: 'Iron (%)', value: 'iron' },
      ],
      desserts: [
        {
          name: 'BELCORP INTERNATIONAL S.A.',
          codOT: '059626',
          descOT: 'CUADERNO (TAPA DURA + 100 HOJAS = + 4 SEP) /// 21.5X16.5 AJUSTE                 ',
          carbs: 24,
          protein: 4.0,
          iron: '1%',
        },
        {
          name: 'CERAMICA LIMA S A',
          codOT: '059638',
          descOT: 'GUIA TURISTICA EL BRUJO (CARATULA + 100 PAG)',
          carbs: 37,
          protein: 4.3,
          iron: '1%',
        },
        {
          name: 'FINANCIERA OH S.A.',
          codOT: '059645',
          descOT: 'BOLSA CHICA',
          carbs: 23,
          protein: 6.0,
          iron: '7%',
        },
        {
          name: 'BANCO PICHINCHA',
          codOT: '059644',
          descOT: 'TACOS X 50 HOJAS IGUALES',
          carbs: 67,
          protein: 4.3,
          iron: '8%',
        },
        {
          name: 'THE CHEESE CORNER S.A.C.',
          codOT: '059627',
          descOT: 'PE-VIV-2100010 VIVITY BROCHURE PACIENTES (8 PAG INC CARAT)',
          carbs: 49,
          protein: 3.9,
          iron: '16%',
        },
        {
          name: 'LABORATORIOS PORTUGAL S R L',
          codOT: '059630',
          descOT: 'STICKER "MARCOL" PARA FRASCO 99ML',
          carbs: 94,
          protein: 0.0,
          iron: '0%',
        },
        {
          name: 'MEDICINA AVANZADA S.A.',
          codOT: '059634',
          descOT: 'BROCHURE (CARÁTULA + 24 PÁGINAS)',
          carbs: 98,
          protein: 0,
          iron: '2%',
        },
        {
          name: 'INVERSIONES PRISCO S.A.C.',
          codOT: '059628',
          descOT: 'RISTRA PRINGLES',
          carbs: 87,
          protein: 6.5,
          iron: '45%',
        },
        {
          name: 'ALCON PHARMACEUTICAL DEL PERU SA',
          codOT: '059649',
          descOT: 'GUIAS  NIFF  (CARÁTULA + 220 PÁGINAS)',
          carbs: 51,
          protein: 4.9,
          iron: '22%',
        },
        {
          name: 'OBRASCON HUARTE LAIN S.A.SUC.DEL PERU',
          codOT: '059646',
          descOT: 'INDIVIDUALES',
          carbs: 65,
          protein: 7,
          iron: '6%',
        },
      ],
    }
  },
}
</script>