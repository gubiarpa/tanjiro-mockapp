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
          // sortable: false,
          value: 'name',
        },
        { text: 'OT', value: 'codOT' },
        { text: 'Descripción', value: 'descOT' },
        { text: 'Status', value: 'status' },
      ],
      desserts: [
        {
          name: 'BELCORP INTERNATIONAL S.A.',
          codOT: '059626',
          descOT: 'CUADERNO (TAPA DURA + 100 HOJAS = + 4 SEP) /// 21.5X16.5 AJUSTE                 ',
          status: 'Hot Melt',
        },
        {
          name: 'CERAMICA LIMA S A',
          codOT: '059638',
          descOT: 'GUIA TURISTICA EL BRUJO (CARATULA + 100 PAG)',
          status: 'Plastificado',
        },
        {
          name: 'FINANCIERA OH S.A.',
          codOT: '059645',
          descOT: 'BOLSA CHICA',
          status: 'Hot Melt',
        },
        {
          name: 'BANCO PICHINCHA',
          codOT: '059644',
          descOT: 'TACOS X 50 HOJAS IGUALES',
          status: 'Hot Melt',
        },
        {
          name: 'THE CHEESE CORNER S.A.C.',
          codOT: '059627',
          descOT: 'PE-VIV-2100010 VIVITY BROCHURE PACIENTES (8 PAG INC CARAT)',
          status: 'Impresión',
        },
        {
          name: 'LABORATORIOS PORTUGAL S R L',
          codOT: '059630',
          descOT: 'STICKER "MARCOL" PARA FRASCO 99ML',
          status: 'Hot Melt',
        },
        {
          name: 'MEDICINA AVANZADA S.A.',
          codOT: '059634',
          descOT: 'BROCHURE (CARÁTULA + 24 PÁGINAS)',
          status: 'Troquelado',
        },
        {
          name: 'INVERSIONES PRISCO S.A.C.',
          codOT: '059628',
          descOT: 'RISTRA PRINGLES',
          status: 'Plasficado',
        },
        {
          name: 'ALCON PHARMACEUTICAL DEL PERU SA',
          codOT: '059649',
          descOT: 'GUIAS  NIFF  (CARÁTULA + 220 PÁGINAS)',
          status: 'Impresión',
        },
        {
          name: 'OBRASCON HUARTE LAIN S.A.SUC.DEL PERU',
          codOT: '059646',
          descOT: 'INDIVIDUALES',
          status: 'Plastificado',
        },
      ],
    }
  },
}
</script>