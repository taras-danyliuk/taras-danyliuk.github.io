<script>
  import { css } from '../css.js';

  export let span = 24;
</script>


<div use:css={{ span }}>
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
        div {
            width: 100%;
        }
    }
</style>
