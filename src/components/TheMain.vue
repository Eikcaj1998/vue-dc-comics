<template>
    <div id="bg-dark">
      <div class="container">
      <h1 > -- Content goes here --</h1>
      </div>
      <div class="navbar">
        <div class="container">
          <div class="row">
            <div class="col" v-for="(img, index) in imgList" :key="index">
                <img :src="require(`../assets/img/buy-${img.imgPath}`)" :href="img.url" alt="img.alt">
                <h3>{{img.text}}</h3>
            </div>
          </div>
        </div>
      </div>
    </div> 
</template>

<script>
export default {
    name: 'TheMain',
    data: function () {
    return {
      imgList: [
        {
          imgPath: "comics-digital-comics.png",
          text:"Digital Comics",
          alt: "digital-comics.png",
          url:"#"
        },
        {
          imgPath: "comics-merchandise.png",
          text:"Dc merchandise",
          alt: "merchandise.png",
          url:"#"
        },
        {
          imgPath: "comics-shop-locator.png",
          text:"Subscription",
          alt: "shop-locator.png",
          url:"#"
        },
        {
          imgPath: "comics-subscriptions.png",
          text:"Comic shop locator",
          alt: "subscriptions.png",
          url:"#"
        },
        {
          imgPath: "dc-power-visa.svg",
          text:"Dc power visa",
          alt: "dc-power-visa.svg",
          url:"#"
        },
      ],
    };
  },
}
</script>

<style lang="scss" scoped>
    #bg-dark {
        background-color: black;
        min-height: 150px;
        h1{
          color:white;
          padding: 35px 0;
        }
    }
    .navbar{
      background-color: #0282F9;
      height: 150px;
      display: flex;
      width: 100%;
      align-items: center;
        .row{
            display: flex;
            justify-content: space-around;
            align-items: center;
          .col{
            display: flex;
            align-items: center;
              img{
                  width: 100%;
                  height: 4rem;
                  width: 3rem;
                  margin-right: 0.8rem;
                }
                h3{
                  text-transform: uppercase;
                  color: white;
                  font-size: 14px;
                }
              }
        }
    }
</style>