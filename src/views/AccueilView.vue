<script>
import card from "../components/Card.vue"
import header1 from "../components/Header.vue"
import footer1 from "../components/Footer.vue"
export default {
    name:"App",
    components: { card, header1, footer1 },
}
</script>

<template class="bg-indigo-25">
    <header1 />
    <div class="text-center mt-14">
        <h1 class="text-4xl leading-10 font-bold">Search properties to rent</h1>
    </div>
    <div class="grid grid-flow-row-dense grid-cols-[repeat(auto-fit,minmax(343px,1fr))]">
        <card class="p-4" 
        :favoris="true"
        image="/images-maison/maison1.jpg" 
        titre="Beverly Springfield"
        lieu="2821 Lake Sevilla, Palm Harbor, TX"
        nbrSDB="2"/>
        <card class="p-4"
        image="/images-maison/maison2.jpg" 
        titre="Palm Harbor"
        lieu="2699 Green Valley, Highland Lake"
        :price="2095" 
        nbrSDB="2"/>
        <card class="p-4"
        image="/images-maison/maison4.jpg" 
        titre="St. Christal"
        lieu="210 US Highway, HighlandLake, FL"
        :price="4650"
        nbrSDB="2"/>
        <card class="p-4"
        :favoris="true" 
        image="/images-maison/maison6.jpg"
        titre="Tarpon Bay" 
        lieu="103 Lake Shores, Michigan, IN"
        :price="4800" 
        nbrSDB="3"/>
        <card class="p-4"
        image="/images-maison/maison3.jpg"
        titre="Faulkner Ave" 
        lieu="909 Woodland St, Michigan, IN"
        :price="4550" 
        nbrSDB="3"/>
        <card class="p-4"
        image="/images-maison/maison5.jpg"
        titre="Cover Red" 
        lieu="243 CurlewRoad, PalmHarbor, TX"
        :price="3100" 
        nbrSDB="2"/>
      
    </div>
    <footer1 />

</template>

