<template>
    <div>
        <h1 class="title is-spaced">Message</h1>
        <h2 class="subtitle">Colored message blocks, to draw attention of your user</h2>
        <hr>

        <div class="columns">
            <div class="column">
                <div class="example">
                    <ex-simple></ex-simple>
                </div>
            </div>
            <div class="column">
                <CodeView :code="ExSimpleCode" />
            </div>
        </div>

        <hr>

        <h2 class="title">Types</h2>

        <div class="columns">
            <div class="column">
                <div class="example">
                    <ex-types></ex-types>
                </div>
            </div>
            <div class="column">
                <CodeView :code="ExTypesCode" />
            </div>
        </div>

        <hr>

        <h2 class="title">Icons</h2>

        <div class="columns">
            <div class="column">
                <div class="example">
                    <ex-icons></ex-icons>
                </div>
            </div>
            <div class="column">
                <CodeView :code="ExIconsCode" />
            </div>
        </div>

        <hr>

        <h2 class="title">Headerless</h2>
        <p class="content">Message without title becomes headerless, they are always non-closable.</p>

        <div class="columns">
            <div class="column">
                <div class="example">
                    <ex-headerless></ex-headerless>
                </div>
            </div>
            <div class="column">
                <CodeView :code="ExHeaderlessCode" />
            </div>
        </div>

        <hr>

        <h2 class="title">Sizes</h2>

        <div class="columns">
            <div class="column">
                <div class="example">
                    <ex-sizes></ex-sizes>
                </div>
            </div>
            <div class="column">
                <CodeView :code="ExSizesCode" />
            </div>
        </div>

        <hr>
        <h2 class="title is-spaced">API</h2>
        <ApiView :data="api" />
    </div>
</template>

<script>
    import api from '@/apis/apiMessage'

    import ExSimple from '@/examples/message/ExSimple'
    import ExSimpleCode from '!!raw-loader!@/examples/message/ExSimple'

    import ExTypes from '@/examples/message/ExTypes'
    import ExTypesCode from '!!raw-loader!@/examples/message/ExTypes'

    import ExIcons from '@/examples/message/ExIcons'
    import ExIconsCode from '!!raw-loader!@/examples/message/ExIcons'

    import ExHeaderless from '@/examples/message/ExHeaderless'
    import ExHeaderlessCode from '!!raw-loader!@/examples/message/ExHeaderless'

    import ExSizes from '@/examples/message/ExSizes'
    import ExSizesCode from '!!raw-loader!@/examples/message/ExSizes'

    export default {
        components: {
            ExSimple,
            ExTypes,
            ExIcons,
            ExHeaderless,
            ExSizes
        },
        data() {
            return {
                api,
                ExSimpleCode,
                ExTypesCode,
                ExIconsCode,
                ExHeaderlessCode,
                ExSizesCode
            }
        }
    }
</script>
