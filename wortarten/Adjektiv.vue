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
                <option value="ao">a-/o-Deklination</option>
                <option value="3kons">Dritte Deklination</option>
            </select>
        </div>

        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_genera" v-html="vocab.descriptors.fb_genera"></label>

            <select name="fb_genera" class="input-disabled" v-model="vocab.fb_genera">
                <option value="1endig">einendig (m/f/n)</option>
                <option value="2endig">zweiendig (m/f)(n)</option>
                <option value="3endig">dreiendig (m)(f)(n)</option>
            </select>
        </div>


        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_komparativ" v-html="vocab.descriptors.fb_komparativ"></label>
            <input type="text" class="input-disabled " v-model="vocab.fb_komparativ">
        </div>

        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_superlativ" v-html="vocab.descriptors.fb_superlativ"></label>
            <input type="text" class="input-disabled " v-model="vocab.fb_superlativ">
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
        name: "adjektive",
        props: ["vocab"],

    }
</script>

<style scoped>

</style>