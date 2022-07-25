<template>
  <footer>
    <div class="container">
    <!-- footer top -->
        <div class="row">
            <div class="col-6">
            <div class="row">
                <div class="col-4">
                    <h4>DC COMICS</h4>
                    <ul>
                        <li><a href="">Characters</a></li>
                        <li><a href="">Comics</a></li>
                        <li><a href="">Movies</a></li>
                        <li><a href="">TV</a></li>
                        <li><a href="">Games</a></li>
                        <li><a href="">Video</a></li>
                        <li><a href="">News</a></li>
                    </ul>
                    <h4>SHOP</h4>
                    <ul>
                        <li><a href="">Shop DC</a></li>
                        <li><a href="">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div class="col-4">
                    <h4>DC</h4>
                    <ul>
                        <li><a href="">Term Of Use</a></li>
                        <li><a href="">Privacy Policy</a></li>
                        <li><a href="">Ad Choices</a></li>
                        <li><a href="">Ad</a></li>
                        <li><a href="">Jobs</a></li>
                        <li><a href="">Subscription</a></li>
                        <li><a href="">Talent Worshops</a></li>
                        <li><a href="">CPSC Certificates</a></li>
                        <li><a href="">Rating</a></li>
                        <li><a href="">Shop Help</a></li>
                        <li><a href="">Contact Us</a></li>
                    </ul>
                </div>
                <div class="col-4">
                    <h4>SITES</h4>
                    <ul>
                        <li><a href="">DC</a></li>
                        <li><a href="">MAD Magazines</a></li>
                        <li><a href="">DC Kids</a></li>
                        <li><a href="">DC Universe</a></li>
                        <li><a href="">DC Power Visa</a></li>
                    </ul>
                </div>
            </div>
        </div>
        <div class="col-6 img-behind">
        </div>
    </div> 
    </div>
    <!-- footer bottom -->
    <div id="bottom-footer">
        <div class="container">
            <div class="d-flex">
                <a href="#" id="sign-up"> SIGN UP NOW</a> 
                <div class="d-flex">
                        <h4 >FOLLOW US</h4>
                        <a href="#"><img src="../assets/img/footer-facebook.png" alt="logo social facebook"></a>
                        <a href="#"><img src="../assets/img/footer-periscope.png" alt="logo social periscope"></a>
                        <a href="#"><img src="../assets/img/footer-pinterest.png" alt="logo social pinterest"></a>
                        <a href="#"><img src="../assets/img/footer-twitter.png" alt="logo social twitter"></a>
                        <a href="#"><img src="../assets/img/footer-youtube.png" alt="logo social youtube"></a>
                </div>
            </div>
        </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'TheFooter'
}
</script>

<style lang="scss" scoped>
    footer {
        background-image:url('../assets/img/footer-bg.jpg');
        background-repeat: no-repeat;
        background-position: right;
        background-size: cover;
        .col-4{padding-top: 40px;}
        h4 {
            color:white;
            margin: 10px 0;
            font-size: 16px;
        }
        ul{
            padding-left: 0;
            li a {
                color:gray;
            font-size: 12px;
            }
        }
        .img-behind{
            background-image: url( '../assets/img/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: center;
        }
        
        //footer-bottom
        #bottom-footer {
            background-color: #343434;
            height: 88px;
            padding: 23px;

            #sign-up {
            
                color: white;
                border: 2px solid dodgerblue;
                padding: 10px;
                transition: 0.7s;
                
                &:hover,
                &:active {
                    background-color: dodgerblue;
                }
            }
            .d-flex {
                display: flex;
                justify-content: space-between;
                align-items: center;
               
               img {
                margin-left: 15px;
                width: 21px;
       
               }
            }
        }
    }
</style>