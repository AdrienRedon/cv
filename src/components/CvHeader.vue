<template>
    <div class="header">
        <h1>Adrien REDON</h1>
        <div class="address"> 
            <ul>
                <li>15 rue des Bienvenus</li>
                <li>69100 Villeurbanne</li>

                <li>Email : redon.adrien@gmail.com</li>
                <li>Tel : 06 48 88 67 61</li>
            </ul>
        </div>
    </div>
</template>

<script>
    
</script>

<style scoped>
    .header {
        display: -webkit-flex;
        display: -moz-flex;
        display: -ms-flex;
        display: -o-flex;
        display: flex;  
        -ms-align-items: center;
        align-items: center;
        justify-content: space-around;
        padding-bottom: 30px;
        border-bottom: 1px solid rgba(0,0,0,0.10);
    }


    .picture {
        margin-left: 100px;
        width: 180px;
        height: 180px;
        border-radius: 50%;
        margin-right: 100px;
    }

    h1 {
        margin-left: 300px;
        flex: 1;
    }

    .address {
        display: -webkit-flex;
        display: -moz-flex;
        display: -ms-flex;
        display: -o-flex;
        display: flex;
        
        text-align: left;
    }

    li {
        display: block; 
        width: 300px;
    }

</style>
