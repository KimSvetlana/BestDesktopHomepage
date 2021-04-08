<template>
    <div class="card-item">
        <div class="card-body">
            <h5 class="card-title">Raisa Moni</h5>
            <h6 class="card-subtitle">Envato Customer</h6>
            <p class="card-text">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore etamet.</p>
        </div>
    </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator'

    @Component
export default class CommentCard extends Vue {}
</script>

<style lang="scss">
.card-item .card-body{
    background: #FFFFFF;
    box-shadow: 0px 4px 20px rgba(0, 70, 156, 0.08);
    border-radius: 5px;
    text-align: start;
    padding-top: 40px;
    padding-left: 30px;
    min-width: 362px;
    min-height: 215px;
}
.card-item .card-title{
    font-weight: 500;
    font-size: 18px;
    line-height: 22px;
    margin-bottom: 15px
}
.card-item .card-subtitle{
    font-size: 14px;
    line-height: 17px;
    color: #999999;
    margin-bottom: 25px;
}
.card-item .card-text{
    line-height: 20px;
}

</style>
