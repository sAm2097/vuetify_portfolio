<template>
 <v-card>
    <v-card-title>Skills</v-card-title>
    <v-list class="mt-5 dotted-list">
        <v-list-item-group>
            Frontend Technologies:
            <v-list-item>
                <v-list-item-content>
                    Vue.js, JavaScript (ES6), TypeScript,
                HTML5/XML, CSS3, Bootstrap, Vuetify, jQuery, React, UX/UI, CI/CD
                </v-list-item-content>
            
            </v-list-item>
        </v-list-item-group>
        <v-list-item-group>
            Backend Technologies:
            <v-list-item>
                <v-list-item-content>
                    Nuxt.js, Node.js, Java, Python, REST-API, MySQL
                </v-list-item-content>
            </v-list-item>
        </v-list-item-group>
        <v-list-item-group>
            Tools:
            <v-list-item>
                <v-list-item-content>
                    Git/Github, Docker, VS Code, WebStorm, Agile/Scrum, Figma
                </v-list-item-content>
            </v-list-item>
        </v-list-item-group>
        <v-list-item-group>
            Languages:
            <v-list-item>
                <v-list-item-content>
                   Languages
                </v-list-item-content>
            </v-list-item>
        </v-list-item-group>
    </v-list>
 </v-card>
</template>

<script>
export default {

}
</script>

<style>
  .dotted-list .v-list-item__content::before {
    content: "\2022";
    margin-right: 0.5em;
    color: #888;
  }
  .scrollable-content {
    max-height: 200px;
    overflow-y: auto;
    overflow-x: hidden;
  }
</style>
