<template>
  <v-container fluid>
    <v-row justify="center">
      <hex-menu
        :items="items"
        rotated
        :wrapperClasses="['page-menu']"
        :svgClasses="['menu-shake']"
        color="var(--menuColor1)"
        activeColor="var(--menuColor2)"
        hoverColor="var(--menuColor2)"
      ></hex-menu>
    </v-row>
    <v-row justify="center" align="center">
      <v-col sm="12" md="9" lg="9" xl="7">
        <h1 class="page-header text-center">About Me</h1>
        <page-article>
          <page-article-section>
            <v-row>
              <v-col cols="12" sm="6">
                <p>
                  Experienced web developer with a demonstrated history of
                  working in the wireless industry. Skilled in PHP, Node.JS,
                  Vue, Angular, HTML, JavaScript, TypeScript, CSS, and SCSS.
                  Strong engineering professional with a Bachelor’s Degree
                  focused in Computer and Information Systems
                  Security/Information Assurance from Dakota State University.
                </p>
              </v-col>
              <v-col cols="12" sm="6">
                <v-row class="me-details">
                  <v-col
                    class="text-center text-sm-right"
                    cols="12"
                    sm="6"
                    lg="3"
                    >Name:</v-col
                  >
                  <v-col
                    class="text-center text-sm-left"
                    cols="12"
                    sm="6"
                    lg="3"
                    >Matt DeKok</v-col
                  >
                  <v-col
                    class="text-center text-sm-right"
                    cols="12"
                    sm="6"
                    lg="3"
                    >Age:</v-col
                  >
                  <v-col
                    class="text-center text-sm-left"
                    cols="12"
                    sm="6"
                    lg="3"
                    >{{ age(new Date(1988, 5, 9)) }}</v-col
                  >
                  <v-col
                    class="text-center text-sm-right"
                    cols="12"
                    sm="6"
                    lg="3"
                    >Location:</v-col
                  >
                  <v-col
                    class="text-center text-sm-left"
                    cols="12"
                    sm="6"
                    lg="3"
                    >Huron, SD</v-col
                  >
                  <v-col
                    class="text-center text-sm-right"
                    cols="12"
                    sm="6"
                    lg="3"
                    >Experience:</v-col
                  >
                  <v-col
                    class="text-center text-sm-left"
                    cols="12"
                    sm="6"
                    lg="3"
                    >{{ age(new Date(2006, 6, 1)) }} years</v-col
                  >
                </v-row>
                <div>&nbsp;</div>
                <h4 class="text-center">
                  <a
                    href="https://www.linkedin.com/in/matt-dekok/"
                    title="LinkedIn"
                    target="_blank"
                  >
                    <svg viewBox="0 0 291 79.459999" class="social-logo">
                      <g transform="translate(-200.55198,-393.96227)">
                        <g
                          transform="matrix(1.018827,0,0,-1.018827,170.5996,498.03288)"
                          id="g3019"
                        >
                          <path
                            d="m 239.3298,95.036 c 0,2.96 2.4604,5.361 5.4956,5.361 l 63.376,0 c 3.0351,0 5.4956,-2.401 5.4956,-5.361 l 0,-64.117 c 0,-2.961 -2.4605,-5.361 -5.4956,-5.361 l -63.376,0 c -3.0352,0 -5.4956,2.4 -5.4956,5.361 l 0,64.117 z"
                            fill="#006699"
                            id="path14"
                          />
                          <path
                            d="m 31.1516,37.709 31.0356,0 0,10.189 -19.8042,0 0,38.874 -11.2314,0 0,-49.063 z"
                            fill="var(--LinkedIn)"
                            id="path16"
                          />
                          <path
                            d="m 77.9001,37.709 0,33.793 -11.2324,0 0,-33.793 11.2324,0 z m -5.6162,38.407 c 3.917,0 6.355,2.595 6.355,5.84 -0.073,3.315 -2.438,5.837 -6.2803,5.837 -3.8428,0 -6.355,-2.522 -6.355,-5.837 0,-3.245 2.4375,-5.84 6.207,-5.84 l 0.073,0 z"
                            fill="var(--LinkedIn)"
                            id="path18"
                          />
                          <path
                            d="m 83.1154,37.709 11.2325,0 0,18.872 c 0,1.01 0.073,2.019 0.3701,2.741 0.8115,2.017 2.6596,4.107 5.7627,4.107 4.0649,0 5.6909,-3.1 5.6909,-7.64 l 0,-18.08 11.2314,0 0,19.377 c 0,10.38 -5.542,15.21 -12.9321,15.21 -6.0591,0 -8.7197,-3.387 -10.1978,-5.694 l 0.075,0 0,4.9 -11.2325,0 c 0.1475,-3.171 0,-33.793 0,-33.793 z"
                            fill="var(--LinkedIn)"
                            id="path20"
                          />
                          <path
                            d="m 133.2487,86.772 -11.2329,0 0,-49.063 11.2329,0 0,10.956 2.8072,3.534 8.7939,-14.49 13.8179,0 -14.7783,20.977 12.9316,14.272 -13.5225,0 c 0,0 -9.2368,-12.769 -10.0498,-14.283 l 0,28.097 z"
                            fill="var(--LinkedIn)"
                            id="path22"
                          />
                          <path
                            d="m 188.7062,51.805 c 0.1475,0.868 0.3697,2.533 0.3697,4.415 0,8.736 -4.4346,17.604 -16.1094,17.604 -12.4888,0 -18.2524,-9.877 -18.2524,-18.835 0,-11.08 7.02,-18 19.2866,-18 4.8774,0 9.3843,0.72 13.0796,2.234 l -1.4785,7.418 c -3.0293,-1.005 -6.1329,-1.507 -9.9751,-1.507 -5.2466,0 -9.8277,2.153 -10.1978,6.743 l 23.2773,-0.07 z m -23.3505,7.599 c 0.2954,2.884 2.2168,7.138 7.02,7.138 5.0976,0 6.2807,-4.543 6.2807,-7.138 l -13.3007,0 z"
                            fill="var(--LinkedIn)"
                            id="path24"
                          />
                          <path
                            d="m 216.801,86.772 0,-16.984 -0.1475,0 c -1.626,2.377 -5.0259,3.963 -9.5322,3.963 -8.6465,0 -16.2573,-6.92 -16.1841,-18.741 0,-10.958 6.8726,-18.094 15.4443,-18.094 4.6553,0 9.0889,2.019 11.3057,5.912 l 0.2222,0 0.4433,-5.119 9.9766,0 c -0.148,2.379 -0.2969,6.488 -0.2969,10.524 l 0,38.539 -11.2314,0 z m 0,-33.421 c 0,-0.864 -0.074,-1.73 -0.2222,-2.45 -0.6641,-3.1 -3.3252,-5.262 -6.5757,-5.262 -4.6557,0 -7.6855,3.748 -7.6855,9.659 0,5.55 2.5869,10.019 7.7588,10.019 3.4726,0 5.9116,-2.378 6.5771,-5.333 0.1475,-0.65 0.1475,-1.371 0.1475,-2.019 l 0,-4.614 z"
                            fill="var(--LinkedIn)"
                            id="path26"
                          />
                          <path
                            d="m 261.8728,37.749 0,33.794 -11.2325,0 0,-33.794 11.2325,0 z m -5.6163,38.408 c 3.917,0 6.355,2.595 6.355,5.838 -0.073,3.316 -2.438,5.839 -6.2807,5.839 -3.8423,0 -6.3545,-2.523 -6.3545,-5.839 0,-3.243 2.4375,-5.838 6.207,-5.838 l 0.073,0 z"
                            fill="#ffffff"
                            id="path28"
                          />
                          <path
                            d="m 268.0881,37.749 11.2324,0 0,18.872 c 0,1.01 0.073,2.019 0.3696,2.741 0.812,2.018 2.6602,4.108 5.7632,4.108 4.0645,0 5.6904,-3.099 5.6904,-7.642 l 0,-18.079 11.2315,0 0,19.377 c 0,10.38 -5.5415,15.21 -12.9316,15.21 -6.0596,0 -8.7198,-3.387 -10.1978,-5.694 l 0.075,0 0,4.901 -11.2324,0 c 0.1474,-3.171 0,-33.794 0,-33.794 z"
                            fill="#ffffff"
                            id="path30"
                          />
                        </g>
                      </g>
                    </svg>
                  </a>
                  <a
                    href="https://github.com/sillvva"
                    title="GitHub"
                    target="_blank"
                  >
                    <svg viewBox="0 0 560 150" class="social-logo">
                      <g
                        transform="matrix(4.16667,0,0,4.16667,74.8679,142.736)"
                      >
                        <path
                          d="M0,-31.904C-8.995,-31.904 -16.288,-24.611 -16.288,-15.614C-16.288,-8.417 -11.621,-2.312 -5.148,-0.157C-4.333,-0.008 -4.036,-0.511 -4.036,-0.943C-4.036,-1.329 -4.05,-2.354 -4.058,-3.713C-8.589,-2.729 -9.545,-5.897 -9.545,-5.897C-10.286,-7.778 -11.354,-8.279 -11.354,-8.279C-12.833,-9.29 -11.242,-9.27 -11.242,-9.27C-9.607,-9.154 -8.747,-7.591 -8.747,-7.591C-7.294,-5.102 -4.934,-5.821 -4.006,-6.237C-3.858,-7.29 -3.438,-8.008 -2.972,-8.415C-6.589,-8.826 -10.392,-10.224 -10.392,-16.466C-10.392,-18.244 -9.757,-19.698 -8.715,-20.837C-8.883,-21.249 -9.442,-22.905 -8.556,-25.148C-8.556,-25.148 -7.188,-25.586 -4.076,-23.478C-2.777,-23.839 -1.383,-24.02 0.002,-24.026C1.385,-24.02 2.779,-23.839 4.08,-23.478C7.19,-25.586 8.555,-25.148 8.555,-25.148C9.444,-22.905 8.885,-21.249 8.717,-20.837C9.761,-19.698 10.392,-18.244 10.392,-16.466C10.392,-10.208 6.583,-8.831 2.954,-8.428C3.539,-7.925 4.06,-6.931 4.06,-5.411C4.06,-3.234 4.04,-1.477 4.04,-0.943C4.04,-0.507 4.333,0 5.16,-0.159C11.628,-2.318 16.291,-8.419 16.291,-15.614C16.291,-24.611 8.997,-31.904 0,-31.904"
                          fill="var(--GitHub)"
                        />
                      </g>
                      <g transform="matrix(1.0738,0,0,1.0738,241.11,84.1613)">
                        <path
                          d="M0,-14.024L-30.267,-14.024C-31.048,-14.024 -31.682,-13.39 -31.682,-12.609L-31.682,2.189C-31.682,2.97 -31.048,3.605 -30.267,3.605L-18.46,3.605L-18.46,21.991C-18.46,21.991 -21.111,22.894 -28.441,22.894C-37.088,22.894 -49.168,19.735 -49.168,-6.829C-49.168,-33.398 -36.589,-36.894 -24.78,-36.894C-14.558,-36.894 -10.154,-35.094 -7.352,-34.227C-6.471,-33.958 -5.657,-34.834 -5.657,-35.615L-2.28,-49.913C-2.28,-50.279 -2.404,-50.719 -2.82,-51.018C-3.958,-51.83 -10.901,-55.715 -28.441,-55.715C-48.646,-55.715 -69.373,-47.118 -69.373,-5.793C-69.373,35.533 -45.643,41.691 -25.646,41.691C-9.089,41.691 0.955,34.616 0.955,34.616C1.369,34.388 1.414,33.809 1.414,33.544L1.414,-12.609C1.414,-13.39 0.781,-14.024 0,-14.024"
                          fill="var(--GitHub)"
                        />
                      </g>
                      <g transform="matrix(1.0738,0,0,1.0738,408.605,125.414)">
                        <path
                          d="M0,-89.181C0,-89.968 -0.624,-90.604 -1.405,-90.604L-18.447,-90.604C-19.226,-90.604 -19.858,-89.968 -19.858,-89.181C-19.858,-89.177 -19.854,-56.246 -19.854,-56.246L-46.418,-56.246L-46.418,-89.181C-46.418,-89.968 -47.045,-90.604 -47.825,-90.604L-64.866,-90.604C-65.641,-90.604 -66.273,-89.968 -66.273,-89.181L-66.273,-0.003C-66.273,0.783 -65.641,1.423 -64.866,1.423L-47.825,1.423C-47.045,1.423 -46.418,0.783 -46.418,-0.003L-46.418,-38.148L-19.854,-38.148C-19.854,-38.148 -19.9,-0.006 -19.9,-0.003C-19.9,0.783 -19.269,1.423 -18.488,1.423L-1.406,1.423C-0.626,1.423 -0.002,0.783 0,-0.003L0,-89.181Z"
                          fill="var(--GitHub)"
                        />
                      </g>
                      <g transform="matrix(1.0738,0,0,1.0738,275.643,42.226)">
                        <path
                          d="M0,-0.008C0,-6.144 -4.92,-11.103 -10.99,-11.103C-17.054,-11.103 -21.977,-6.144 -21.977,-0.008C-21.977,6.122 -17.054,11.095 -10.99,11.095C-4.92,11.095 0,6.122 0,-0.008"
                          fill="var(--GitHub)"
                        />
                      </g>
                      <g transform="matrix(1.0738,0,0,1.0738,274.334,81.2007)">
                        <path
                          d="M0,22.36L0,-18.805C0,-19.586 -0.63,-20.225 -1.41,-20.225L-18.398,-20.225C-19.178,-20.225 -19.875,-19.422 -19.875,-18.64L-19.875,40.337C-19.875,42.069 -18.795,42.585 -17.397,42.585L-2.091,42.585C-0.412,42.585 0,41.76 0,40.309L0,22.36Z"
                          fill="var(--GitHub)"
                        />
                      </g>
                      <g transform="matrix(1.0738,0,0,1.0738,478.153,128.907)">
                        <path
                          d="M0,-64.519L-16.911,-64.519C-17.687,-64.519 -18.318,-63.88 -18.318,-63.093L-18.318,-19.367C-18.318,-19.367 -22.615,-16.223 -28.713,-16.223C-34.811,-16.223 -36.429,-18.99 -36.429,-24.961L-36.429,-63.093C-36.429,-63.88 -37.059,-64.519 -37.835,-64.519L-54.999,-64.519C-55.773,-64.519 -56.408,-63.88 -56.408,-63.093L-56.408,-22.074C-56.408,-4.339 -46.524,0 -32.927,0C-21.771,0 -12.777,-6.163 -12.777,-6.163C-12.777,-6.163 -12.35,-2.915 -12.155,-2.53C-11.962,-2.146 -11.457,-1.758 -10.911,-1.758L0.008,-1.806C0.782,-1.806 1.417,-2.446 1.417,-3.23L1.411,-63.093C1.411,-63.88 0.779,-64.519 0,-64.519"
                          fill="var(--GitHub)"
                        />
                      </g>
                      <g transform="matrix(1.0738,0,0,1.0738,520.624,45.52)">
                        <path
                          d="M0,61.379C-5.866,61.2 -9.845,58.539 -9.845,58.539L-9.845,30.298C-9.845,30.298 -5.92,27.892 -1.104,27.462C4.986,26.917 10.854,28.756 10.854,43.284C10.854,58.603 8.206,61.627 0,61.379M6.67,11.134C-2.935,11.134 -9.468,15.42 -9.468,15.42L-9.468,-14.778C-9.468,-15.565 -10.098,-16.201 -10.874,-16.201L-27.965,-16.201C-28.742,-16.201 -29.373,-15.565 -29.373,-14.778L-29.373,74.4C-29.373,75.187 -28.742,75.827 -27.963,75.827L-16.105,75.827C-15.571,75.827 -15.167,75.551 -14.868,75.069C-14.573,74.59 -14.148,70.958 -14.148,70.958C-14.148,70.958 -7.16,77.58 6.069,77.58C21.601,77.58 30.508,69.702 30.508,42.214C30.508,14.726 16.282,11.134 6.67,11.134"
                          fill="var(--GitHub)"
                        />
                      </g>
                      <g transform="matrix(1.0738,0,0,1.0738,326.929,109.556)">
                        <path
                          d="M0,-46.64L-12.784,-46.64C-12.784,-46.64 -12.803,-63.525 -12.803,-63.529C-12.803,-64.168 -13.132,-64.488 -13.872,-64.488L-31.292,-64.488C-31.969,-64.488 -32.333,-64.189 -32.333,-63.538L-32.333,-46.086C-32.333,-46.086 -41.063,-43.979 -41.653,-43.808C-42.241,-43.638 -42.674,-43.096 -42.674,-42.449L-42.674,-31.482C-42.674,-30.694 -42.044,-30.057 -41.265,-30.057L-32.333,-30.057L-32.333,-3.673C-32.333,15.923 -18.587,17.848 -9.312,17.848C-5.073,17.848 -0.003,16.487 0.834,16.178C1.34,15.992 1.635,15.468 1.635,14.9L1.649,2.835C1.649,2.048 0.984,1.411 0.236,1.411C-0.509,1.411 -2.415,1.714 -4.377,1.714C-10.656,1.714 -12.784,-1.205 -12.784,-4.984C-12.784,-8.761 -12.785,-30.057 -12.785,-30.057L0,-30.057C0.779,-30.057 1.411,-30.694 1.411,-31.482L1.411,-45.219C1.411,-46.006 0.779,-46.64 0,-46.64"
                          fill="var(--GitHub)"
                        />
                      </g>
                    </svg>
                  </a>
                </h4>
              </v-col>
            </v-row>
          </page-article-section>
          <page-article-section>
            <v-row>
              <v-col>
                <div class="text-center">
                  <p>Like and want to support my work? No problem!</p>
                  <p>
                    <v-btn to="/donate">Buy me a sandwich</v-btn>
                  </p>
                </div>
              </v-col>
            </v-row>
          </page-article-section>
        </page-article>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts">
import HexMenu from "@/components/hex-menu/hex-menu-svg.vue";
import PageArticle from "@/components/page-article/page-article.vue";
import PageArticleSection from "@/components/page-article/page-article-section.vue";
import PageArticleSectionItems from "@/components/page-article/page-article-section-items.vue";
import PageArticleSectionItem from "@/components/page-article/page-article-section-item.vue";

export default {
  components: {
    HexMenu,
    PageArticle,
    PageArticleSection,
    PageArticleSectionItems,
    PageArticleSectionItem,
  },
  head() {
    return {
      title: "About Me",
    };
  },
  data() {
    return {
      items: [
        { link: "/", label: "Intro" },
        { link: "/about", label: "About Me" },
        { link: "/experience", label: "Experience" },
        { link: "/skills", label: "Skills" },
        { link: "/projects", label: "Projects" },
      ],
    };
  },
  methods: {
    age(birthday: Date) {
      const ageDifMs = Date.now() - birthday.getTime();
      const ageDate = new Date(ageDifMs); // miliseconds from epoch
      return Math.abs(ageDate.getUTCFullYear() - 1970);
    },
  },
};
</script>

<style lang="scss" scoped>
.me-details {
  margin: 0 -10px;
  > div {
    padding: 5px 10px;
    &:nth-child(2n-1) {
      font-weight: 600;
    }
    @media (max-width: 600px) {
      &:nth-child(2n-1) {
        padding-bottom: 0;
      }
      &:nth-child(2n) {
        padding-top: 2px;
      }
    }
  }
}

.social-logo {
  height: 24px;
  margin: 0 10px;
}
</style>
