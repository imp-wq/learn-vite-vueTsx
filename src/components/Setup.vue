
<script lang="tsx">
import { defineComponent } from "@vue/runtime-core"
const fn = (e: Event) => {
    console.log('click')
}
const list = ['aaa', 'bbbb', 'cccccc']

export default defineComponent({
    setup() {
        return () =>
        (<>
            <h2>Setup </h2>
            < button onClick={fn} > btn </button>
            <ul>
                {list.map(item => <li>{item}</li>)}
            </ul>
        </>
        )

    }
})
</script>

<style>
</style>