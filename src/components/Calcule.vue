<template>
    <v-row class="mx-0 px-0 bg-primary pt-16 pb-16">
        <v-col cols="12" sm="6" md="6">
            <h1 class="text-sm-h4 font-weight-bold pl-4 text-md-h2">Cansado de pagar conta de energia?</h1>
            <h3 class="text-secondary font-weight-light text-sm-h5 pl-4 px-3" :class="smAndDown ? '' : 'mt-3'"><span
                    class="font-weight-bold">Calcule sua
                    economia
                    de
                    dinheiro</span> em energia elétrica</h3>

            <v-form v-model="valid" align="center">
                <v-container class="py-8">
                    <v-row>
                        <v-col cols="12" sm="12" md="12">
                            <v-text-field v-model="nome" :rules="nomeRules" label="Nome" color="secondary"
                                hint="Seu nome"></v-text-field>
                        </v-col>

                        <v-col cols="12" sm="12" md="12">
                            <v-text-field v-model="Email" :rules="emailRules" label="Email"
                                placeholder="email@email.com.br" hint="Seu e-mail" color="secondary"></v-text-field>
                        </v-col>

                        <v-col cols="12" sm="12" md="12">
                            <v-text-field v-model="WhatsApp" :rules="WhatsAppRules" label="WhatsApp" color="secondary"
                                hint="Seu whatsapp"></v-text-field>
                        </v-col>

                        <v-col cols="12" sm="12" align="center" :class="smAndDown ? '' : 'mt-16'">
                            <v-btn class="rounded-pill mb-2 bg-secondary w-100 h-100 text-sm-h6 font-weight-bold">
                                CALCULAR MINHA ECONOMIA
                            </v-btn>
                            <h6 class="font-weight-regular">Ou <a class="text-secondary" href="">clique aqui</a> para
                                falar com um
                                atendente pelo WhatsApp</h6>
                        </v-col>
                    </v-row>
                </v-container>
            </v-form>
        </v-col>

        <v-col cols="12" sm="6">
            <v-img class="h-100 rounded-xl mx-2" cover
                src="https://files.axshare.com/gsc/124I4K/a8/f4/a1/a8f4a175254a4ad8b5176535a0a201e8/images/lp-v040a/u96.svg?pageId=0e8f7217-3d97-461b-a799-1d997c56f49f" />
        </v-col>
    </v-row>
</template>

<script setup>
import { ref } from 'vue';
import { useDisplay } from 'vuetify';

const { smAndDown } = useDisplay()

const valid = ref(false);

const nome = ref('');
const nomeRules = ref([
    value => {
        if (value) return true;
        return 'É necessário inserir um Nome.';
    },
    value => {
        if (value?.length <= 50) return true;
        return 'Insira um nome de no minimo 3 letras.';
    },
]);

const Email = ref('');
const emailRules = ref([
    value => {
        if (value) return true;
        return 'É necessário inserir um E-mail.';
    },
    value => {
        if (/.+@.+\..+/.test(value)) return true;
        return 'E-mail deve ser válido.';
    },
]);

const WhatsApp = ref('');
const WhatsAppRules = ref([
    value => {
        if (value) return true;
        return 'É necessário inserir um Número';
    },
    value => {
        if (/.+@.+\..+/.test(value)) return true;
        return 'O número deve ser válido.';
    },
]);
</script>