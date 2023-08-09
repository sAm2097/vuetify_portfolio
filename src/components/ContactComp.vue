<template>
  <v-col cols="12" sm="12" class="px-16" id="contact">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="child">
              <h1>Contact info.</h1>
              <v-btn
                icon="fas fa-map-marker-alt"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <span class="text-caption">74394 Hessigheim, Germany </span
              ><br />
              <v-btn
                icon="fas fa-phone-alt"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <span class="text-caption">+49 178 9806278 </span> <br />
              <span class="text-caption">+91 9000 995998 </span> <br />
              <v-btn
                icon="fas fa-envelope"
                color=""
                class="mt-10"
                variant="outlined"
              ></v-btn
              ><br />
              <a class="text-caption" href = "mailto: sumanth.anugandula97@gmail.com">sumanth.anugandula97@gmail.com</a><br />
              <a class="text-caption" href = "mailto: samanugandula1518@gmail.com">samanugandula1518@gmail.com</a><br />
             
            </div>
          </v-col>
          <v-col cols="12" sm="8">
            <h1 class="mt-8">Send your message</h1>
            <v-divider></v-divider>
            <span class="text-caption"
              >Please, use this form to send the message or find the links in footer section.</span
            >
            <v-row class="mt-10">
              <v-col cols="12" sm="6">
                <v-text-field
                  label="Name"
                  v-model="name"
                  persistent-hint
                  variant="outlined"
                ></v-text-field>
              </v-col>
              <v-col cols="12" sm="6">
                <v-text-field
                  label="Phone No"
                  v-model="phone"
                  persistent-hint
                  variant="outlined"
                ></v-text-field>
              </v-col>
            </v-row>
            <v-textarea
              label="Message"
              v-model="message"
              persistent-hint
              variant="outlined"
            ></v-textarea>
            <v-btn color="#FBDF7E" class="mt-2" @click="submitForm">Submit Now</v-btn>
          </v-col>
        </v-row>
      </v-col>

</template>

<script>
export default {
data(){
  return {
    name:'',
    phone:'',
    message:''
  }
},
methods:{
  submitForm(){
   alert('Please use the Email to send message')
  }
}
}
</script>

<style>

</style>