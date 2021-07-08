<template>
  <div id="crew">
    <v-container fluid>
      <component-title text="Kadra" />

      <v-row class="mt-10" align="start" justify="center" no-gutters>
        <v-col cols="12" lg="10" md="10">
          <v-row class="mt-10" align="start" justify="center" no-gutters>
            <v-col
              cols="6"
              lg="2"
              md="3"
              sm="4"
              v-for="(item, index) in crew"
              :key="index"
            >
              <crew-card
                :name="item.name"
                :faculty="item.faculty"
                :avatar="item.avatar"
              />
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import CrewCard from "./CrewCard";
import ComponentTitle from "@/components/ComponentTitle";
export default {
  name: "Crew",
  components: { ComponentTitle, CrewCard },
  data() {
    return {
      crew: [
        {
          name: "Marcin Sylka",
          faculty: "WIMiFT",
          avatar: "question.png"
        },
        {
          name: "Ula Sadowska",
          faculty: "WILiT",
          avatar: "question.png"
        },
        {
          name: "Natalia Fedko",
          faculty: "WA",
          avatar: "question.png"
        },
        {
          name: "Hubert Ziętowski",
          faculty: "WARiE",
          avatar: "Hubert.jpg"
        },
        {
          name: "Laura Strojna",
          faculty: "WARiE",
          avatar: "Laura.jpg"
        },
        {
          name: "Szymon Bujanowski",
          faculty: "WARiE",
          avatar: ""
        },
        {
          name: "Witold Rozumek",
          faculty: "WARiE",
          avatar: "Wiciu.jpg"
        },
        {
          name: "Bartosz Cieślewicz",
          faculty: "WIiT",
          avatar: "Bartus.jpg"
        },
        {
          name: "Kornelia Kostrzewska",
          faculty: "WIiT",
          avatar: "Nela.jpg"
        },
        {
          name: "Martyna Kurz",
          faculty: "WIiT",
          avatar: "Kurz.jpg"
        },
        {
          name: "Bartosz Kruczynski",
          faculty: "WILiT",
          avatar: "Kruczynski.jpeg"
        },
        {
          name: "Daria Wstawska",
          faculty: "WILiT",
          avatar: "Daria.jpg"
        },
        {
          name: "Katarzyna Chmielewska",
          faculty: "WILiT",
          avatar: "Kaska.jpg"
        },
        {
          name: "Mikołaj Gemzicki",
          faculty: "WILiT",
          avatar: "Beton.jpg"
        },
        {
          name: "Aleksandra Stróżyk",
          faculty: "WIM",
          avatar: "Olcia.jpg"
        },
        {
          name: "Magdalena Kubiak",
          faculty: "WIM",
          avatar: "Madzia.jpg"
        },
        {
          name: "Magdalena Wojtczak",
          faculty: "WIM",
          avatar: "Wojtczak.jpg"
        },
        {
          name: "Martyna Maćkowiak",
          faculty: "WIM",
          avatar: "Martini.jpg"
        },
        {
          name: "Paweł Dzięcioł",
          faculty: "WIM",
          avatar: "Dzieciol.jpg"
        },
        {
          name: "Patryk Ginter",
          faculty: "WIMiFT",
          avatar: "Gynter.jpg"
        },
        {
          name: "Wojciech Gindera",
          faculty: "WIŚiE",
          avatar: "Gindera.jpg"
        },
        {
          name: "Dagmara Maćkowiak",
          faculty: "WIZ",
          avatar: "Daga.jpeg"
        },
        {
          name: "Maria Zienkiewicz",
          faculty: "WIZ",
          avatar: "Marysia.jpg"
        },
        {
          name: "Karolina Ławniczak",
          faculty: "WIZ",
          avatar: "Kala.jpg"
        },
        {
          name: "Marta Kocurek",
          faculty: "WTCh",
          avatar: "Kocur.jpg"
        },
        {
          name: "Weronika Frankiewicz",
          faculty: "WTCh",
          avatar: "Werka.jpg"
        },
        {
          name: "Wiktoria Stachowicz",
          faculty: "WTCh",
          avatar: "Wika.jpg"
        }
      ]
    };
  }
};
</script>

<style scoped></style>
