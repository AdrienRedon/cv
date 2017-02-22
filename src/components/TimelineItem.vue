<template>
    <li class="block">
        <div class="timeline-date">
            <slot name="date"></slot>
        </div>
        <div class="timeline"></div>
        <div class="item">
           <slot></slot>
        </div>
    </li>
</template>

<script>
    
</script>

<style scoped>
    .block {
        display: -webkit-flex;
        display: -moz-flex;
        display: -ms-flex;
        display: -o-flex;
        display: flex;
        align-items: center;
        position: relative;
        padding: 26px 0;
    }

    .block:before {
        content: '';
        position: absolute;
        top: 0;
        left: 150px;
        height: 100%;
        width: 4px;
        background: #ECECEC;
    }

    .timeline {
        z-index: 2;
        top: 0;
        left: 0;
        width: 20px;
        height: 20px;
        margin: 0 20px;
        border-radius: 50%;
        background: #FAD250;
        border: 2px solid #FFFFFF;
        box-shadow: 0 2px 0 0 rgba(0,0,0,0.20), inset 0 1px 0 0 rgba(0,0,0,0.10);

        overflow: hidden;
    }

    .timeline-date {
        width: 120px;
        border-radius: 50%;

        letter-spacing: 0;
    }

    .item {
        flex: 1;
        display: block;
        margin-right: 20px;
        padding: 7px;
        padding-right: 10px;
        background-color: #fff;
        box-shadow: 0 1px 1px 1px rgba(0,0,0,0.20);
        border-radius: 2px 2px 5px 5px;
        border-bottom: 3px solid #F3F5FA;
        display: -webkit-flex;
        display: -moz-flex;
        display: -ms-flex;
        display: -o-flex;
        display: flex;
    }


    h2 {
        text-transform: uppercase;
        font-size: 0.7rem;
        margin: 0px;
        color: #4D4F53;
    }

    p {
        text-align: left;
        margin: 0;
        font-weight: 200;
        margin-top: 5px;
    }
</style>