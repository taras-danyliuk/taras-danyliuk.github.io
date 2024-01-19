<script>
  import { css } from '../css.ts';

  export let span = 24;
  export let justifyContent = "flex-start";
  export let alignItems = "flex-start";
  export let responsive = true;
</script>


<div
        style="justify-content: {justifyContent}; align-items: {alignItems}"
        use:css={{ span }}
        class:responsive={responsive}
>
    <slot/>
</div>


<style>
    div {
        padding: 0 12px;
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        width: calc(100% / 24 * var(--span));
    }

    @media (max-width: 750px) {
        .responsive {
            width: 100%;
        }
    }
</style>
