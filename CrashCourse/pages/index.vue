<template>
  <div>
    <div class="container">
      <Hero/>
      <LargeCardDisplay v-for="cardInfo in largeCardInfo" :key="cardInfo.id" :cardsSection="cardInfo" />
      <SmailCardDisplay v-for="cardInfo in smailCardInfo" :key="cardInfo.id" :cardsSection="cardInfo" />
    </div>
  </div>
</template>

<script>
import {largeCardSections,smallCardSections } from "@/assets/data.js"
export default {
  data(){
    return {
      largeCardInfo:largeCardSections,
      smailCardInfo:smallCardSections,
    }
  }
}
</script>
 

 <<style scoped>
 
 </style>