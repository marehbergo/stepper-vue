<template>
  <div class="home">
    <v-stepper v-model="e1">
      <v-stepper-header>
        <v-stepper-step :complete="e1 > 1" step="1">Categoria</v-stepper-step>
        <v-divider></v-divider>
        <v-stepper-step :complete="e1 > 2" step="2">Atividades</v-stepper-step>
        <v-divider></v-divider>
        <v-stepper-step :complete="e1 > 3" step="3">Dados</v-stepper-step>
        <v-divider></v-divider>
        <v-stepper-step :complete="e1 > 4" step="4">Pagamento</v-stepper-step>
      </v-stepper-header>

      <v-stepper-items>
        <v-stepper-content step="1">
          <v-card
            class="mb-5"
            color="grey lighten-1"
            height="200px"
          ></v-card>

          <v-layout row wrap justify-space-between>
            <v-flex xs6>
            </v-flex>
            
            <v-flex xs6 text-xs-right>
              <v-btn
                color="primary"
                @click="e1 = 2"
              > Próximo
              </v-btn>
            </v-flex>
          </v-layout>
        </v-stepper-content>

        <v-stepper-content step="2">
          <v-card
            class="mb-5"
            color="grey lighten-1"
            height="200px"
          ></v-card>

          <v-layout row wrap justify-space-between>
            <v-flex xs6>
              <v-btn
                flat
                @click="e1 = 1"
              > Voltar
              </v-btn>
            </v-flex>
            
            <v-flex xs6 text-xs-right>
              <v-btn
                color="primary"
                @click="e1 = 3"
              > Próximo
              </v-btn>
            </v-flex>
          </v-layout>
        </v-stepper-content>

        <v-stepper-content step="3">
          <v-card
            class="mb-5"
            color="grey lighten-1"
            height="200px"
          ></v-card>

          <v-layout row wrap justify-space-between>
            <v-flex xs6>
              <v-btn
                flat
                @click="e1 = 2"
              > Voltar
              </v-btn>
            </v-flex>
            
            <v-flex xs6 text-xs-right>
              <v-btn
                color="primary"
                @click="e1 = 4"
              > Próximo
              </v-btn>
            </v-flex>
          </v-layout>
        </v-stepper-content>

        <v-stepper-content step="4">
          <v-card
            class="mb-5"
            color="grey lighten-1"
            height="200px"
          ></v-card>

          <v-layout row wrap justify-space-between>
            <v-flex xs6>
              <v-btn
                flat
                @click="e1 = 3"
              > Voltar
              </v-btn>
            </v-flex>
            
            <v-flex xs6 text-xs-right>
              <v-btn
                color="primary"
                @click="e1 = 1"
              > Finalizar
              </v-btn>
            </v-flex>
          </v-layout>
        </v-stepper-content>
      </v-stepper-items>
    </v-stepper>    
  </div>
</template>

<script>
  export default {
    name: 'Stepper',
    data () {
      return {
        e1: 0
      }
    }
  }
</script>
