<script lang="ts">
    import type {Bird} from './game';
    export let bird:Bird;
</script>


<style>
  #bird{
      border:solid black 1px;
      position: absolute;
      border-radius: 6px; 
      background-color:#F8D800;
      
  }
</style>

<section
style="width:{bird.size}px; height:{bird.size}px; top:{bird.top}px;left:{bird.left}px" id="bird"
></section>