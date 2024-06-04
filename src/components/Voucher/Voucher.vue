<script>
export default {
    name: "Voucher"
}
</script>

<template>
    <div class="voucher">
        <i class="voucher__gift" />
        <img class="voucher__img" src="./i/voucher-pic.png" alt="voucher-picture" />
        <div class="voucher__wrap">
            <p class="voucher__title">Это твой билет в Пекин!</p>
            <p class="voucher__text">
                Сделай заказ доставки от 1999₽<br>
                с 6.06 по 18.09 и стань участником конкурса
                с крутыми подарками от Kimchi и партнёров. Подробнее в разделе «Акции»
            </p>
        </div>
    </div>
</template>

<style scoped>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.voucher {
    position: relative;
    width: 355px;
    height: 106px;
    display: flex;
    align-items: center;
    overflow: hidden;
}

.voucher__img {
    width: 80px;
    height: 100%;
    background: #fff;
    border-top-left-radius: 8px;
    border-bottom-left-radius: 8px;
    border: 1px dashed #46bf73;
    border-right: none;
}
.voucher__wrap {
    position: relative;
    background: #e9f9f2;
    height: 100%;
    text-align: left;
    gap: 5px;
    padding: 11px 25px 11px 17px;
    border-top-right-radius: 8px;
    border-bottom-right-radius: 8px;
    border: 1px dashed #46bf73;
    border-left: none;
    text-wrap: balance;
}

.voucher__wrap:before {
    content: "";
    width: 18px;
    height: 18px;
    border-radius: 50%;
    background: #fff;
    position: absolute;
    top: -10px;
    left: -10px;
    border: 1px dashed #46bf73;
}

.voucher__wrap:after {
    content: "";
    width: 18px;
    height: 18px;
    border-radius: 50%;
    background: #fff;
    position: absolute;
    bottom: -10px;
    left: -10px;
    border: 1px dashed #46bf73;
}

.voucher__title {
    font-family: "SF Pro Display", sans-serif;
    font-size: 17px;
    font-weight: 400;
    line-height: 22.1px;
    letter-spacing: 0.01em;
    color: #000;
    margin-bottom: 2px;
}

.voucher__text {
    font-family: "SF Pro Display", sans-serif;
    font-size: 11px;
    font-weight: 400;
    line-height: 14.85px;
    letter-spacing: 0.01em;
    color: #1DBF73;
}

.voucher__gift {
    width: 15px;
    height: 16px;
    position: absolute;
    top: 11px;
    right: 12px;
    background-image: url(i/gift.svg);
    background-repeat: no-repeat;
    background-position: 50% 50%;
    z-index: 1;
}

</style>