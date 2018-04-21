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
            <label class="label-disabled" for="fb_dklasse" v-html="vocab.descriptors.fb_dklasse"></label>
            <select name="fb_kklasse" class="input-disabled" v-model="vocab.fb_dklasse">
                <option value="">Keine Angabe</option>
                <option value="a">a-Deklination</option>
                <option value="o">o-Deklination</option>
                <option value="e">e-Deklination</option>
                <option value="u">u-Deklination</option>
                <option value="3kons">Dritte Deklination</option>
                <option value="indekl">indeklinabel</option>
            </select>
        </div>

        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_genus" v-html="vocab.descriptors.fb_genus"></label>
            <select name="fb_kklasse" class="input-disabled" v-model="vocab.fb_genus">
                <option value="">Keine Angabe</option>
                <option value="mask">maskulin</option>
                <option value="fem">feminin</option>
                <option value="neutr">neutral</option>
                <option value="commune">substantivum commune</option>
            </select>
        </div>



        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_bes_numerus" v-html="vocab.descriptors.fb_bes_numerus"></label>

            <select name="fb_bes_numerus" class="input-disabled" v-model="vocab.fb_bes_numerus">
                <option value="0">Nein</option>
                <option value="">Nein</option>
                <option value="sgtantum">Sg. tantum</option>
                <option value="pltantum">Pl. tantum</option>
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
        name: "nomina",
        props: ["vocab"],
    }
</script>

<style scoped>

</style>