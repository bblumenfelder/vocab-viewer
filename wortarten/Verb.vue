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
            <label class="label-disabled" for="fb_kklasse" v-html="vocab.descriptors.fb_kklasse"></label>

            <select name="fb_kklasse" id="" class="input-disabled" v-model="vocab.fb_kklasse">
                <option value="">Keine Angabe</option>
                <option value="a">a-Konjugation</option>
                <option value="e">e-Konjugation</option>
                <option value="i">i-Konjugation</option>
                <option value="k">kons. Konjugation</option>
                <option value="ki">kons. Konjugation (+i)</option>
            </select>
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_1pssgpr" v-html="vocab.descriptors.fb_1pssgpr"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.fb_1pssgpr">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_1pssgpf" v-html="vocab.descriptors.fb_1pssgpf"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.fb_1pssgpf">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_hat_ppp" v-html="vocab.descriptors.fb_hat_ppp"></label>
            <input type="hidden" class="hidden" name="fb_hat_ppp" id="fb_hat_ppp_2" value="0" v-model="vocab.fb_hat_ppp">
            <input type="checkbox" name="fb_hat_ppp" id="fb_hat_ppp"
                   class="input-disabled"
                   v-model="vocab.fb_hat_ppp"
                   value="1"
                   disabled="disabled">

        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_hat_ppp" v-html="vocab.descriptors.fb_hat_pfa"></label>
            <input type="checkbox" name="fb_hat_pfa" id="fb_hat_pfa"
                   v-model="vocab.fb_hat_pfa"
                   class="input-disabled"

                   value="1"
                   disabled="disabled">
            <input type="hidden" class="hidden" name="fb_hat_pfa" id="fb_hat_pfa_2" value="0" v-model="vocab.fb_hat_pfa">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_ppp" v-html="vocab.descriptors.fb_ppp"></label>
            <input type="text" class="input-disabled  serif" v-model="vocab.fb_ppp">
        </div>
        <div class="flex-group-sb form-group-50">
            <label class="label-disabled" for="fb_pfa" v-html="vocab.descriptors.fb_pfa"></label>
            <input type="text" class="input-disabled serif" v-model="vocab.fb_pfa">
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
        name: "verben",
        props: ["vocab"],
    }
</script>

<style scoped>

</style>