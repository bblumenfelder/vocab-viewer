<template>
    <div class="vocab-viewer flex-group-sb">
        <div class="vocab-viewer__vocab-data"
             :class="{'col-50':this.morph_json, 'w-100': !this.morph_json}">

            <adjektiv v-if="this.data.wortart=='adjektiv'" :vocab="data"></adjektiv>
            <nomen v-if="this.data.wortart=='nomen'" :vocab="data"></nomen>
            <numerale v-if="this.data.wortart=='numerale'" :vocab="data"></numerale>
            <partikel v-if="this.data.wortart=='partikel'" :vocab="data"></partikel>
            <pronomen v-if="this.data.wortart=='pronomen'" :vocab="data"></pronomen>
            <verb v-if="this.data.wortart=='verb'" :vocab="data"></verb>

        </div>
        <div v-if="this.morph_json" class="vocab-viewer__morph"
             :class="{'col-50':this.morph_json}">
            <json-vuer :json="this.morph_json"></json-vuer>
        </div>
    </div>
</template>

<script>
    import JsonVuer from '../json-vuer/json-vuer'
    import Adjektiv from './wortarten/Adjektiv'
    import Nomen from './wortarten/Nomen'
    import Numerale from './wortarten/Numerale'
    import Partikel from './wortarten/Partikel'
    import Pronomen from './wortarten/Pronomen'
    import Verb from './wortarten/Verb'

    export default {
        name: "vocab-viewer",
        props: ['data'],
        data: function () {
            return {
                'morph_json': JSON.parse(this.data.morph),
            };
        },
        components: {
            'json-vuer': JsonVuer,
            'adjektiv': Adjektiv,
            'nomen': Nomen,
            'numerale': Numerale,
            'partikel': Partikel,
            'pronomen': Pronomen,
            'verb': Verb,
        },
    }
</script>

<style scoped>
    .vocab-viewer {

        background: #fff;
    }

    .vocab-viewer__morph {
        padding: 1rem
    }

    .vocab-viewer__vocab-data {
        padding: 1rem
    }
</style>
