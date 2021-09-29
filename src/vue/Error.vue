
<script>
    export default {
        props: {
            error: {
                type: String,
                required: true
            }
        }
    };
</script>

<style lang="sass" scoped>
    @import "../css/variables"
    .panel
        background-color: $error
        color: $text-opposite
        a, a:visited, a:hover
            text-decoration: underline
            color: $text-opposite
</style>
