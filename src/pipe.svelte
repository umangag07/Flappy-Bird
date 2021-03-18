<script lang="ts">
    import type {PipePair} from './game';
    export let pipe:PipePair;
</script>

<style>
    .pipe{
         position: absolute;
         
         background: linear-gradient(90deg, #fcff9e 0%, #c67700 100%);
    }
</style>

{#if pipe.show}
<section style="left:{pipe.left}px;
                top:{pipe.topPipe.top}px;
                width:{pipe.width}px;
                height:{pipe.topPipe.height}px;"
                class="top-pipe pipe">
</section>
<section style="left:{pipe.left}px;
                top:{pipe.bottomPipe.top}px;
                width:{pipe.width}px;
                height:{pipe.bottomPipe.height}px;"
                class="bottom-pipe pipe">
</section>

{/if}