<template>
  <b-container class="bv-example-row">
    <b-row>
      <b-col>
        <b-card title="Közzétételi lista" tag="article" class="mb-2">
          <b-card-text>
            <div>
              <b-button
                block
                v-for="link in links"
                :key="link.url"
                :href="link.url"
                target="_blank"
                variant="primary"
                class="mb-2"
                >{{ link.desc }}</b-button
              >
            </div>
          </b-card-text>
        </b-card>
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          url: "/downloads/BÁI_Szülői tájékoztató_2022.pdf",
          desc: "Beiratkozás",
        },
        {
          url: "http://www.kir.hu/kir2int/IntezmenyKereso/Intezmeny/Index/033463",
          desc: "Adatok a kir.hu oldalon",
        },
        {
          url: "https://kir2info.kir.hu/pub/Index/033463",
          desc: "Közzétételi lista a kir.hu oldalon",
        },
        {
          url: "/downloads/szmsz.pdf",
          desc: "Szervezeti és működési szabályzat",
        },
        { url: "/downloads/Házirend.pdf", desc: "Házirend" },
        { url: "/downloads/Pedagógiai program.pdf", desc: "Pedagógiai program" },
      ],
    };
  },
};
</script>
