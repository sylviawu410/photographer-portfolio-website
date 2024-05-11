<template>
  <div>
    <TheHeader />
    <Nuxt />
    <TheFooter />
  </div>
</template>
  
<script>
import TheHeader from "~/components/TheHeader";
import TheFooter from "~/components/TheFooter";

export default {
  components: {
    TheHeader,
    TheFooter,
  },
};
</script>

<style>
@media screen and (min-width: 992px) {
  body {
    font-family: Manrope;
    background: var(--Dark-03, #070708);
    font-size: 14px;
    font-style: normal;
    font-weight: 400;
    color: white;
    line-height: 27px;
    flex-shrink: 0;
    /* margin:auto; */
    margin-block-start: 0;
    margin-block-end: 0;
  }
  
  h1 {
    color: var(--Absolute-White, #FFF);
    font-size: 49px;
    font-weight: 600;
    line-height: normal;
    text-transform: uppercase;
    margin: 0;

  }


}




@media screen and (min-width: 1440px) {
  body {
    font-size: 18px;
  }
}
</style>