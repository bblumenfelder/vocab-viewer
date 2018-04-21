<template>
    <div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="id" v-html="vocab.descriptors.id"></label>
            <input type="text" class="input-disabled " v-model="vocab.id">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="zahlenwert" v-html="vocab.descriptors.zahlenwert"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.zahlenwert">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="lemma" v-html="vocab.descriptors.lemma"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.lemma">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="info" v-html="vocab.descriptors.info"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.info">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="lemma_ordinal" v-html="vocab.descriptors.lemma_ordinal"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.lemma_ordinal">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="lemma_distributiv" v-html="vocab.descriptors.lemma_distributiv"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.lemma_distributiv">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="lemma_multiplikativ" v-html="vocab.descriptors.lemma_multiplikativ"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.lemma_multiplikativ">
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
        name: "numeralia",
        props: ["vocab"],

    }
</script>

<style scoped>

</style>