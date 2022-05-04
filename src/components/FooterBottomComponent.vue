<template>
    <div class="bottom">
       <div class="container">
           <div class="row">
               <div class="col">
                   <div class="sign_up">
                       <button>sign-up now!</button>
                   </div>
               </div>
               <div class="col">
                   <div class="follow">
                       <h3>follow us</h3>
                       <div class="icon">
                           <img src="@/assets/img/footer-facebook.png" alt="">
                           <img src="@/assets/img/footer-twitter.png" alt="">
                           <img src="@/assets/img/footer-youtube.png" alt="">
                           <img src="@/assets/img/footer-pinterest.png" alt="">
                           <img src="@/assets/img/footer-periscope.png" alt="">
                       </div>
                   </div>
               </div>
           </div>
       </div>
    </div>
</template>

<script>
export default {
    name:'FooterBottomComponent'
}
</script>

<style lang="scss" scoped>

.bottom{
    background-color: $bgFooter;
    padding: 1.5rem 0;
    .sign_up{
        
        button{
            background-color: transparent;
            border: 1px solid $primaryColor;
            padding: 1rem;
            text-transform: uppercase;
            color: $white;
            font-weight: 700;
        }
    }
    .follow{
        display: flex;
        align-items: center;
        padding: 0.5rem;
        justify-content: flex-end;
        h3{
            color: $primaryColor;
            margin-right: 1.5rem;
            text-transform: uppercase;
        }
        img{
            margin-right: 1rem;
        }
    }
}
</style>