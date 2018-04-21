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
            <label class="label-disabled" for="fb_art" v-html="vocab.descriptors.fb_art"></label>
            <select name="fb_art" class="input-disabled" v-model="vocab.fb_art">
                <option value="s" >Keine Angabe</option>
                <option value="pers" >Personalpronomen</option>
                <option value="poss" >Possessivpronomen</option>
                <option value="demo" >Demonstrativpronomen</option>
                <option value="rel" >Relativpronomen</option>
                <option value="interrog" >Interrogativpronomen</option>
                <option value="indef" >Indefinitpronomen</option>
            </select>
        </div>


        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_wortart" v-html="vocab.descriptors.fb_wortart"></label>
            <select name="fb_wortart" class="input-disabled" v-model="vocab.fb_wortart">
                <option value="">Keine Angabe</option>
                <option value="adj">adjektivisch</option>
                <option value="subst">substantivisch</option>
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
        name: "pronomen",
        props: ['vocab']
    }
</script>

<style scoped>

</style>