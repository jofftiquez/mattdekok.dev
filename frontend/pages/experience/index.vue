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
      <v-col sm="10" md="9" lg="7">
        <h1 class="page-header text-center">Experience</h1>
        <page-article>
          <page-article-section>
            <h2>Work Experience</h2>
            <page-article-section-items>
              <page-article-section-item image="images/ddb.png">
                <h3>Forum, Twitch, and Discord Moderator</h3>
                <h4>
                  <a href="https://www.dndbeyond.com/" title="DND Beyond">
                    D&amp;D Beyond
                  </a>
                </h4>
                <h5>2019 - Present</h5>
              </page-article-section-item>
              <page-article-section-item image="images/valmont.jpg">
                <h3>Front End Web Developer</h3>
                <h4>
                  <a
                    href="http://www.valmont.com/"
                    title="Valmont Industries, Inc."
                  >
                    Valmont Industries, Inc.
                  </a>
                </h4>
                <h5>2019 - Present</h5>
              </page-article-section-item>
              <page-article-section-item image="images/agsense.png">
                <h3>Web Developer</h3>
                <h4>
                  <a href="http://agsense.com/" title="AgSense, LLC.">
                    AgSense, LLC.
                  </a>
                </h4>
                <h5>2012 - Present</h5>
              </page-article-section-item>
            </page-article-section-items>
          </page-article-section>
          <page-article-section>
            <h2>Education</h2>
            <page-article-section-items>
              <page-article-section-item image="images/dsu.png">
                <h3>
                  Computer and Information Systems Security/Information
                  Assurance
                </h3>
                <h4>
                  <a
                    href="https://dsu.edu/academics/degrees-and-programs/computer-information-systems-bs"
                    title="Dakota State University"
                  >
                    Dakota State University
                  </a>
                </h4>
                <h5>Bachelor of Science Degree</h5>
              </page-article-section-item>
              <page-article-section-item image="images/mti.png">
                <h3>Computer Software and Media Applications</h3>
                <h4>
                  <a
                    href="https://www.mitchelltech.edu/academics/programs-we-offer/online/administrative-office-specialist"
                    title="Mitchell Technical Institute"
                  >
                    Mitchell Technical Institute
                  </a>
                </h4>
                <h5>Associate's Degree</h5>
              </page-article-section-item>
            </page-article-section-items>
          </page-article-section>
          <page-article-section>
            <h2>Licenses & Certifications</h2>
            <page-article-section-items>
              <page-article-section-item image="images/mos.png">
                <h3>Microsoft Office Specialist</h3>
                <h4>Microsoft Excel - Mitchell Tech</h4>
                <h5>
                  <a
                    href="https://www.microsoft.com/en-us/learning/dashboard.aspx"
                  >
                    Credential ID 6154048
                  </a>
                </h5>
              </page-article-section-item>
              <page-article-section-item image="images/udemy.svg">
                <h3>
                  <a
                    href="https://www.udemy.com/react-the-complete-guide-incl-redux/"
                  >
                    React - The Complete Guide
                  </a>
                </h3>
                <h4>Udemy - Academind by Maximilian Schwarzmülle</h4>
                <h5>
                  <a target="_blank" href="http://ude.my/UC-WSZBKXEW">
                    Certificate
                  </a>
                </h5>
              </page-article-section-item>
              <page-article-section-item image="images/udemy.svg">
                <h3>
                  <a
                    href="https://www.udemy.com/course/understanding-typescript/"
                  >
                    Understanding TypeScript
                  </a>
                </h3>
                <h4>Udemy - Academind by Maximilian Schwarzmülle</h4>
                <h5>
                  <a target="_blank" href="http://ude.my/UC-DIDRRWV8">
                    Certificate
                  </a>
                </h5>
              </page-article-section-item>
              <page-article-section-item image="images/udemy.svg">
                <h3>
                  <a href="https://www.udemy.com/nuxtjs-vuejs-on-steroids/">
                    Nuxt.js - Vue.js on Steroids
                  </a>
                </h3>
                <h4>Udemy - Academind by Maximilian Schwarzmülle</h4>
                <h5>
                  <a target="_blank" href="http://ude.my/UC-T5TFG77X">
                    Certificate
                  </a>
                </h5>
              </page-article-section-item>
            </page-article-section-items>
          </page-article-section>
        </page-article>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
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
      title: "Experience",
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
};
</script>
