<template>
    <div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="id" v-html="vocab.descriptors.id">ID</label>
            <input type="text" class="input-disabled " v-model="vocab.id">
        </div>

        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="lemma" v-html="vocab.descriptors.lemma">Lemma</label>
            <input type="text" class="input-disabled  serif" v-model="vocab.lemma">
        </div>

        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="getInfo" v-html="vocab.descriptors.getInfo">Zusatzinformationen</label>
            <input type="text" class="input-disabled " v-model="vocab.getInfo">
        </div>

        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_stamm" v-html="vocab.descriptors.fb_stamm"></label>
            <input type="text" class="input-disabled " v-model="vocab.fb_stamm">
        </div>


        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_art" v-html="vocab.descriptors.fb_art"></label>
            <select name="fb_kklasse" class="input-disabled" v-model="vocab.fb_art">
                <option value="" >Keine Angabe</option>
                <option value="adv" >Adverb</option>
                <option value="praep" >Präposition</option>
                <option value="konj" >Konjunktion</option>
                <option value="interj" >Interjektion</option>
                <option value="anderes" >unbestimmt</option>
            </select>
        </div>


        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="bedeutung" v-html="vocab.descriptors.bedeutung"></label>
            <input type="text" class="input-disabled " v-model="vocab.bedeutung">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="bedeutungen_alle" v-html="vocab.descriptors.bedeutungen_alle"></label>
            <textarea rows="10" class="input-disabled " v-model="vocab.bedeutungen_alle"></textarea>
        </div>
    </div>
</template>

<script>
    export default {
        name: "partikel",
        props: ['vocab']
    }
</script>

<style scoped>

</style>