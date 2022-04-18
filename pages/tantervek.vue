<template>
  <b-container class="bv-example-row">
    <b-row>
      <b-col>
        <b-card
          v-for="(tanterv,  index) in tantervek"
          :key="tanterv.title"
          :title="tanterv.title"
          tag="article"
          class="mb-2"
        >
          <b-card-text>
            <div v-for="tantargy in tanterv.tantargyak" :key="tantargy.label">
              <h5 class="mt-4 ml-3">{{ tantargy.label }}</h5>
              <b-nav vertical>
                <b-nav-item
                class=" ml-3"
                  v-for="sublink in tantargy.items"
                  :key="sublink.label"
                  :href="sublink.url"
                  target="_blank"
                  >{{ sublink.label }}</b-nav-item
                >
              </b-nav>
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
      tantervek: {
        also: {
          title: "Helyi tantárgyi tantervek alsó tagozat",

          tantargyak: [
   
            {
              label: "Digitális kultúra",
              items: [
                {
                  label: "Digitális kultúra 3-4",
                  url: "/downloads/tantervek/Digitalis kultúra 3-4..pdf",
                }
              ],
            },
            {
              label: "Ének-zene",
              items: [
                {
                  label: "Ének-zene 1-2",
                  url: "/downloads/tantervek/Ének-zene 1-2..pdf",
                },
                {
                  label: "Ének-zene 3-4",
                  url: "/downloads/tantervek/Ének-zene 3-4..pdf",
                }
              ],
            },
            {
              label: "Etika",
              items: [
                {
                  label: "Etika 1-2",
                  url: "/downloads/tantervek/Etika 1-2..pdf",
                },
                {
                  label: "Etika 3-4",
                  url: "/downloads/tantervek/Etika 3-4..pdf",
                }
              ],
            },

    
            {
              label: "Környezetismeret",
              items: [
                {
                  label: "Környezetismeret 3-4",
                  url: "/downloads/tantervek/Környezetismeret 3-4..pdf",
                },
              ],
            },
            {
              label: "Magyar nyelv és irodalom",
              items: [
                {
                  label: "Magyar nyelv és irodalom 1-2",
                  url: "/downloads/tantervek/Magyar nyelv és irodalom 1-2..pdf",
                },
                {
                  label: "Magyar nyelv és irodalom 3-4",
                  url: "/downloads/tantervek/Magyar nyelv és irodalom 3-4..pdf",
                },
              ],
            },
   
            {
              label: "Matematika",
              items: [
                {
                  label: "Matematika 1-2",
                  url: "/downloads/tantervek/Matematika 1-2..pdf",
                },
                {
                  label: "Matematika 3-4",
                  url: "/downloads/tantervek/Matematika 3-4..pdf",
                }
              ],
            },
            {
              label: "Német nemzetiségi nyelv",
              items: [
                {
                  label: "Német nemzetiségi nyelv 1-8",
                  url: "/downloads/tantervek/Német nemzetiségi nyelv 1-8..pdf",
                },
              ],
            },
            {
              label: "Technika és tervezés",
              items: [
                {
                  label: "Technika és tervezés 1-2",
                  url: "/downloads/tantervek/Technika és tervezés 1-2..pdf",
                },
                {
                  label: "Technika és tervezés 3-4",
                  url: "/downloads/tantervek/Technika és tervezés 3-4..pdf",
                }
              ],
            },
           
            {
              label: "Testnevelés",
              items: [
                {
                  label: "Testnevelés 1-2",
                  url: "/downloads/tantervek/Testnevelés 1-2..pdf",
                }
              ],
            }
          ],
        },
        felso: {
          title: "Helyi tantárgyi tantervek felső tagozat",

          tantargyak: [
            {
              label: "Biológia",
              items: [
                {
                  label: "Biológia 8.",
                  url: "/downloads/tantervek/Biológia 8.osztály.pdf",
                },
              ],
            },
            {
              label: "Digitális kultúra",
              items: [
   
                {
                  label: "Digitális kultúra 5",
                  url: "/downloads/tantervek/Digitális-kultúra-5.-évfolyam.pdf",
                },
                {
                  label: "Digitális kultúra 6",
                  url: "/downloads/tantervek/Digitális-kultúra-6.-évfolyam.pdf",
                },
              ],
            },
            {
              label: "Ének-zene",
              items: [
  
                {
                  label: "Ének-zene 5-6",
                  url: "/downloads/tantervek/Ének-zene 5-6..pdf",
                },
                {
                  label: "Ének-zene 7-8",
                  url: "/downloads/tantervek/Ének-zene 7-8..pdf",
                },
              ],
            },
            {
              label: "Etika",
              items: [
   
                {
                  label: "Etika 5-8",
                  url: "/downloads/tantervek/Etika 5-8..pdf",
                },
              ],
            },
            {
              label: "Fizika",
              items: [
                {
                  label: "Fizika 7",
                  url: "/downloads/tantervek/Fizika 7..pdf",
                },
                {
                  label: "Fizika 8",
                  url: "/downloads/tantervek/Fizika 8..pdf",
                },
              ],
            },
            {
              label: "Irodalom",
              items: [
                {
                  label: "Irodalom 5",
                  url: "/downloads/tantervek/Irodalom 5..pdf",
                },
                {
                  label: "Irodalom 6",
                  url: "/downloads/tantervek/Irodalom 6..pdf",
                },
                {
                  label: "Irodalom 7-8",
                  url: "/downloads/tantervek/Irodalom 7-8..pdf",
                },
              ],
            },
 
 
            {
              label: "Magyar nyelv",
              items: [
                {
                  label: "Magyar nyelv 5-6",
                  url: "/downloads/tantervek/Magyar-nyelv 5-6..pdf",
                },
                {
                  label: "Magyar nyelv 7-8",
                  url: "/downloads/tantervek/Magyar-nyelv  7-8..pdf",
                },
              ],
            },
            {
              label: "Matematika",
              items: [
      
                {
                  label: "Matematika 5-6",
                  url: "/downloads/tantervek/Matematika 5-6..pdf",
                },
                {
                  label: "Matematika 7-8",
                  url: "/downloads/tantervek/Matematika 7-8..pdf",
                },
              ],
            },
            {
              label: "Német nemzetiségi nyelv",
              items: [
                {
                  label: "Német nemzetiségi nyelv 1-8",
                  url: "/downloads/tantervek/Német nemzetiségi nyelv 1-8..pdf",
                },
              ],
            },
            {
              label: "Technika és tervezés",
              items: [
   
                {
                  label: "Technika és tervezés 5",
                  url: "/downloads/tantervek/Technika és tervezés 5..pdf",
                },
                {
                  label: "Technika és tervezés 6",
                  url: "/downloads/tantervek/Technika és tervezés 6..pdf",
                },
                {
                  label: "Technika és tervezés 7",
                  url: "/downloads/tantervek/Technika és tervezés 7..pdf",
                },
              ],
            },
            {
              label: "Természetismeret",
              items: [
                {
                  label: "Természetismeret 5",
                  url: "/downloads/tantervek/Természetismeret 5..pdf",
                },
                {
                  label: "Természetismeret 6",
                  url: "/downloads/tantervek/Természetismeret 6..pdf",
                },
              ],
            },
            {
              label: "Testnevelés",
              items: [
    
                {
                  label: "Testnevelés 5",
                  url: "/downloads/tantervek/Testnevelés 5..pdf",
                },
                {
                  label: "Testnevelés 6",
                  url: "/downloads/tantervek/Testnevelés 6..pdf",
                },
                {
                  label: "Testnevelés 7",
                  url: "/downloads/tantervek/Testnevelés 7..pdf",
                },
                {
                  label: "Testnevelés 8",
                  url: "/downloads/tantervek/Testnevelés 8..pdf",
                },
              ],
            },
            {
              label: "Történelem",
              items: [
                {
                  label: "Történelem 5-8",
                  url: "/downloads/tantervek/Történelem 5-8..pdf",
                },
              ],
            },
          ],
        },
      },
    };
  },
};
</script>
