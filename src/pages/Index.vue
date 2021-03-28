<template>
  <q-page style="background-color: #E5E4E2">
    <div class="" style="background-color:yellow">
      <div class="q-mx-sm">
        <q-carousel
          animated
          swipeable
          v-model="slide"
          arrows
          navigation
          infinite
          height="200px"
        >
          <q-carousel-slide :name="1" img-src="https://cdn.quasar.dev/img/mountains.jpg" />
          <q-carousel-slide :name="2" img-src="https://cdn.quasar.dev/img/parallax1.jpg" />
          <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax2.jpg" />
          <q-carousel-slide :name="4" img-src="https://cdn.quasar.dev/img/quasar.jpg" />
        </q-carousel>
      </div>
    </div>

    <div class="row justify-between q-mx-md q-my-md">
      <div class="col justify-between q-mx-md q-my-md">
        <q-btn round color="white" icon="qr_code_2" text-color="black" size="20px"/>
        <p style="font-size: 12px"> Pagar com código QR </p>
      </div>

      <div class="col justify-between q-mx-md q-my-md">
        <q-btn round color="white" icon="sell" text-color="black" size="20px"/>
        <p style="font-size: 12px"> Ofertas do dia </p>
      </div>

      <div class="col justify-between q-mx-md q-my-md">
        <q-btn round color="white" icon="shopping_basket" text-color="black" size="20px"/>
        <p style="font-size: 12px"> Supermercado </p>
      </div>

      <div class="col justify-between q-mx-md q-my-md">
        <q-btn round color="white" icon="drive_eta" text-color="black" size="20px"/>
        <p style="font-size: 12px"> Carros, motos e outros </p>
      </div>

      <div class="col justify-between q-mx-md q-my-md">
        <q-btn round color="white" icon="add" text-color="black" size="20px"/>
        <p style="font-size: 12px"> Ver mais </p>
      </div>
    </div>

    <div>
      <q-card class="q-mx-sm">
        <q-card-section>
          <div>
            <p class="text-h6"> Visto recentemente </p>
            <q-separator grey/>
          </div>
          <div>
            <q-img src="https://cdn.quasar.dev/img/parallax2.jpg" basic/>
          </div>
        </q-card-section>

        <div class="row q-mx-md">
          <p>Fusível Cerâmico 4a X 250v /5x20mm/com Retardo - Kit 3pçs</p>
        </div>

        <div class="row q-mx-md">
          <p class="text-h6" style="bold">R$ 23,75</p>
        </div>

        <q-separator dark />

        <div>
          <q-card-actions>
            <q-btn flat align="between" class="full-width" text-color="blue" icon-right="arrow_right" label="Ver histórico de navegação"/>
          </q-card-actions>
        </div>
      </q-card>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      slide: 1
    }
  }
}
</script>
