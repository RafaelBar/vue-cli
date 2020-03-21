<template>
    <div class="col-sm-6 col-md-4">
        <div class="panel panel-default">
            <div class="panel-body quote">
                <slot></slot>
            </div>
        </div>
    </div>
</template>

<script>
export default {
   
}
</script>

<style lang="scss" scoped>
    .panel-body{
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        font-size: 24px;
        color: #6e6e6e;
        &.quote{
            cursor: pointer;
            &:hover{
                background-color: #ffe2e2;
            }
        }
    } 
</style>