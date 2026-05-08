<script lang="ts">

    interface Props {
        page: string;
    }
    
    const {page}: Props = $props();

</script>

<p class="pt-2">You are here: {page}</p>