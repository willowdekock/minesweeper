<script>
    export let status;

    function emojiOf(status) {
        switch(status) {
            case 'win':
                return '😎';
            case 'lose':
                return '🤯';
            default:
                return '🙂';
        }
    }

    $: emoji = emojiOf(status);
</script>

<span class="smiley">{ emoji }</span>

<style>
    .smiley {
        font-size: 64px;
        padding: 5px;
    }
</style>