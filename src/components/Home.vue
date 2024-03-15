<template>

  <v-row class="mx-0 px-0">
    <v-col class="bg-primary pt-16" align="center">

      <h5 class="text-secondary font-weight-regular text-sm-h5">VOCÊ SABIA?</h5>

      <h4 class="font-weight-regular pt-3 px-5 text-sm-h4">
        O <span class="text-secondary">sol potiguar</span> é perfeito pra produzir a energia da sua casa ou empresa</h4>

      <v-col cols="12" sm="11" md="11" class="mb-n16 justify-center" align="center" justify="center">
        <v-img class="mt-10 mx-2"
          src="https://files.axshare.com/gsc/124I4K/a8/f4/a1/a8f4a175254a4ad8b5176535a0a201e8/images/lp-v040a/u13.svg?pageId=0e8f7217-3d97-461b-a799-1d997c56f49f" />
      </v-col>
    </v-col>
  </v-row>

  <v-row class="mx-0 px-0">
    <v-col align="center" class="mt-16">
      <h4 class="text-terciary text-sm-h4">Quer saber quanto você economizaria?
      </h4>
      <h6 class="font-weight-regular text-terciary text-sm-h6" style="font-size: 10px;">
        Dica: alguns casos economizam até 95% na conta de energia!
      </h6>

      <v-btn class="bg-yellow mt-5 rounded-pill w-75 h-50 text-sm-h5 font-weight-bold">
        CALCULAR ECONOMIA
      </v-btn>

      <h6 class="mt-2 font-weight-regular text-terciary text-sm-h6">
        LEVA APENAS 1 MINUTO PARA SOLICITAR
      </h6>
    </v-col>
  </v-row>

  <Motivos />
  <Calcule />
  <Bonus />
</template>


<script setup>
import Motivos from '@/components/Motivos.vue'
import Calcule from '@/components/Calcule.vue'
import Bonus from '@/components/Bonus.vue'
</script>