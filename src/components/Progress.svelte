<script>
    export let className = "";
    export let width = 0;
</script>

<div class="holder {className}">
    <div class="value" style="width: {width}%"/>
</div>

<style>
    .holder {
        width: 100%;
        height: 6px;
        border-radius: 3px;
        background-color: rgba(255,255,255,0.3);
        overflow: hidden;
    }

    .value {
        height: 100%;
        background-color: #fff;
    }
</style>
