<template>
    <div>
        <div class = "main-wrapper">
            <div class = "container">
                <div class = "product-div">
                    <div class = "product-div-left">
                        <div class = "img-container">
                            <img src = "../../imgs/services-house/house1.jpg" alt = "watch">
                        </div>
                        <div class = "hover-container">
                            <div><img src = "../../imgs/services-house/house2.jpg"></div>
                            <div><img src = "../../imgs/services-house/house3.jpg"></div>
                            <div><img src = "../../imgs/services-house/house4.jpg"></div>
                        </div>
                    </div>
                    <div class = "product-div-right">
                        <span class = "product-name">House Cleaning</span>
                        <span class = "business-name">Locaverse <img src="https://www.locaverse.at/icons/verified-icon.svg" alt=""></span>
                        <div class = "product-rating">
                            <span><i class = "fas fa-star"><font-awesome-icon :icon="['fas','star']"/></i></span>
                            <span><i class = "fas fa-star"><font-awesome-icon :icon="['fas','star']"/></i></span>
                            <span><i class = "fas fa-star"><font-awesome-icon :icon="['fas','star']"/></i></span>
                            <span><i class = "fas fa-star"><font-awesome-icon :icon="['fas','star']"/></i></span>
                            <span><i class = "fas fa-star-half-alt"><font-awesome-icon :icon="['fas','star-half-alt']"/></i></span>
                            <span>(450 ratings)</span>
                        </div>
                        <p class = "product-description">House cleaning service involves a team of professionals meticulously tidying, sanitizing, and organizing homes. They handle dusting, vacuuming, mopping, bathroom and kitchen cleaning, ensuring a fresh, welcoming, and hygienic living environment for clients.</p>
                        <div class = "btn-groups">
                            <button type = "button" class = "add-cart-btn"><i class = "fas fa-shopping-cart"></i>add to cart</button>
                            <button type = "button" class = "buy-now-btn"><i class = "fas fa-wallet"></i>buy now</button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

html, body{
    font-family: 'Roboto', sans-serif;
}

.main-wrapper{
    min-height: 100vh;
    background-color: #f1f1f1;
    display: flex;
    align-items: center;
    justify-content: center;
}
.container{
    max-width: 1200px;
    padding: 0 1rem;
    margin: 0 auto;
}
.product-div{
    margin: 1rem 0;
    padding: 2rem 0;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    background-color: #fff;
    border-radius: 3px;
    column-gap: 10px;
}
.product-div-left{
    padding: 20px;
}
.product-div-right{
    padding: 20px;
}
.img-container img{
    max-width: 480px;
    margin: 0 auto;
}
.hover-container{
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    margin-top: 32px;
}
.hover-container div{
    border: 2px solid #2196f3;
    padding: 1rem;
    border-radius: 3px;
    margin: 0 4px 8px 4px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.active{
    border-color: #2196f3!important;
}
.hover-container div:hover{
    border-color: #2196f3;
}
.hover-container div img{
    max-width: 100px;
    cursor: pointer;
}
.product-div-right span{
    display: block;
}
.product-name{
    font-size: 26px;
    margin-bottom: 15px;
    font-weight: 700;
    letter-spacing: 1px;
    opacity: 0.9;
}
.business-name{
    color: #2196f3;
    font-size: 20px;
    line-height: 1.6;
    margin-bottom: 0;
}
.product-rating{
    display: flex;
    align-items: center;
    margin-top: 12px;
}
.product-rating span{
    margin-right: 6px;
}
.product-rating i {
    color: #FF9F00;
}
.product-description{
    font-weight: 18px;
    line-height: 1.6;
    font-weight: 300;
    opacity: 0.9;
    margin-top: 22px;
}
.btn-groups{
    margin-top: 130px;
}
.btn-groups button{
    display: inline-block;
    font-size: 16px;
    font-family: inherit;
    text-transform: uppercase;
    padding: 15px 16px;
    color: #fff;
    cursor: pointer;
    transition: all 0.3s ease;
}
.btn-groups button .fas{
    margin-right: 8px;
}
.add-cart-btn{
    background-color: #FF9F00;
    border: 2px solid #FF9F00;
    margin-right: 8px;
}
.add-cart-btn:hover{
    background-color: #fff;
    color: #FF9F00;
}
.buy-now-btn{
    background-color: #000;
    border: 2px solid #000;
}
.buy-now-btn:hover{
    background-color: #fff;
    color: #000;
}

@media screen and (max-width: 992px){
    .product-div{
        grid-template-columns: 100%;
    }
    .product-div-right{
        text-align: center;
    }
    .product-rating{
        justify-content: center;
    }
    .product-description{
        max-width: 400px;
        margin-right: auto;
        margin-left: auto;
    }
}

@media screen and (max-width: 400px){
    .btn-groups button{
        width: 100%;
        margin-bottom: 10px;
    }
}
</style>
