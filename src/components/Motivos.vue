<template>
    <v-row class="mt-16 bg-quartiary mx-0 px-0 pt-8 pb-8" justify="center" align="center"
        :class="smAndDown ? '' : 'pt-16 pb-16 mt-16'">
        <v-col cols="6" sm="6" md="5" :class="smAndDown ? '' : 'pt-16'">
            <h5 class="text-terciary font-weight-regular text-sm-h4 text-md-h3"><span
                    class="font-weight-bold">Principais
                    motivos</span> para
                instalar energia solar</h5>

            <div class="d-flex justify-space mt-4" :class="smAndDown ? '' : 'w-75 mt-16'">
                <v-col cols="4" sm="3" md="3" class="bg-primary d-flex justify-center align-center rounded-lg h-50">
                    <h4 class="text-secondary text-sm-h4 text-md-h3">1</h4>
                </v-col>

                <h6
                    class="ml-2 text-terciary font-weight-regular d-flex justify-center align-center text-sm-h6 text-md-h5">
                    Reduz
                    até 95% na
                    conta de
                    luz</h6>
            </div>

            <div class="d-flex justify-space mt-4" :class="smAndDown ? '' : 'w-75 mt-16'">
                <v-col cols="4" sm="3" md="3" class="bg-primary d-flex justify-center align-center rounded-lg h-50">
                    <h4 class="text-secondary text-sm-h4 text-md-h3">2</h4>
                </v-col>

                <h6
                    class="ml-2 text-terciary font-weight-regular d-flex justify-center align-center text-sm-h6 text-md-h5">
                    Valoriza seu
                    imóvel</h6>
            </div>

            <div class="d-flex justify-space mt-4" :class="smAndDown ? '' : 'w-75 mt-16'">
                <v-col cols="4" sm="3" md="3" class="bg-primary d-flex justify-center align-center rounded-lg h-50">
                    <h4 class="text-secondary text-sm-h4 text-md-h3">3</h4>
                </v-col>

                <h6
                    class="ml-2 text-terciary font-weight-regular d-flex justify-center align-center text-sm-h6 text-md-h5">
                    Sem
                    surpresas ou
                    taxas
                    extras em sua conta de energia</h6>
            </div>

            <div class="d-flex justify-space mt-4" :class="smAndDown ? '' : 'w-75 mt-16'">
                <v-col cols="4" sm="3" md="3" class="bg-primary d-flex justify-center align-center rounded-lg h-50">
                    <h4 class="text-secondary text-sm-h4 text-md-h3">4</h4>
                </v-col>

                <h6
                    class="ml-2 text-terciary font-weight-regular d-flex justify-center align-center text-sm-h6 text-md-h5">
                    Colabora com o
                    meio
                    ambiente</h6>
            </div>
        </v-col>

        <v-col cols="6">
            <v-img class="rounded-xl" :class="smAndDown ? 'h-100' : 'h-75'"
                src="https://files.axshare.com/gsc/124I4K/a8/f4/a1/a8f4a175254a4ad8b5176535a0a201e8/images/lp-v040a/u95.svg?pageId=0e8f7217-3d97-461b-a799-1d997c56f49f" />
        </v-col>
    </v-row>
</template>

<script setup>
import { useDisplay } from 'vuetify';

const { smAndDown } = useDisplay()
</script>