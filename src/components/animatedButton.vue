<template>
    <div class="round">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
    </div>
</template>

<script>
export default {   

}
</script>

<style scoped>
.round {
    position: relative;
    border: 3px solid #fff;
    width: 100px;
    height: 100px;
    border-radius: 100%;
}

span {
    z-index: 999;
    height: 3px;
    margin:1px;
    width: 30px;
    background: #fff;
    transition: 0.4s ease;
}

span:first-child {
    display: block;
    position: absolute;
    transform: rotate(-45deg);
    left: 25%;
    bottom: 35%;
}

span:nth-child(2) {
    display: block;
    position: absolute;
    transform: rotate(-45deg);
    left: 45%;
    bottom: 35%;
}

span:nth-child(3) {
    display: block;
    position: absolute;
    transform: rotate(45deg);
    left: 25%;
    bottom: 54%;
}

span:nth-child(4) {
    display: block;
    position: absolute;
    transform: rotate(45deg);
    left: 45%;
    bottom: 54%;
}

.round:hover span:nth-child(1) {
    transform: rotate(-225deg);
}

.round:hover span:nth-child(2) {
    transform: rotate(-225deg);
}

.round:hover span:nth-child(3) {
    transform: rotate(225deg);
}

.round:hover span:nth-child(4) {
    transform: rotate(225deg);
}
</style>
