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
        border:1px solid #dddddd;
        margin: 15px 0;
        padding: 15px;
        &.quote{
            cursor: pointer;
            &:hover{
                background-color: #127bff;
                color:#fff;
            }
        }
    } 
</style>