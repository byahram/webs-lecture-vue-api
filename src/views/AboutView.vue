<template>
  <HeaderCont />
  <TitleCont name1="about" name2="Api" />
  <section className="about__cont">
    <div className="container">
      <div className="about__inner"></div>
    </div>
  </section>
  <ContactCont />
  <FooterCont />
</template>

<script>
import HeaderCont from "@/components/HeaderCont.vue";
import FooterCont from "@/components/FooterCont.vue";
import TitleCont from "@/components/TitleCont.vue";
import ContactCont from "@/components/ContactCont.vue";

export default {
  components: {
    HeaderCont,
    FooterCont,
    TitleCont,
    ContactCont,
  },
};
</script>

<style scoped lang="scss">
.about__cont {
  background-color: var(--black);
}

.about__inner {
  .about {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding-bottom: 30vh;
    color: var(--white);
    font-family: var(--kor_font);

    .about__img {
      flex: 0 0 64%;
    }

    .about__txt {
      flex: 0 0 32%;
      text-align: justify;

      h3 {
        margin-bottom: 30px;
        font-size: 1.4rem;
        line-height: 1;
      }

      p {
        font-size: 1rem;
        line-height: 1.6;
      }
    }

    &:nth-child(even) {
      flex-direction: row-reverse;
    }
  }
}
</style>
