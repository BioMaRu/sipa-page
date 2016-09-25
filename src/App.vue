<template>
    <div id="app">
        <navbar placement="top" type="default">
            
            <!-- Brand as slot -->
            <li><a href="/" title="Home">Shopping with Newtron</a></li>
            <li><a href="/" title="Home">Checkout</a></li>
            <li><a href="/" title="Home">Cart</a></li>
            <li><a href="/" title="Home">My account</a></li>
            
            <a slot="brand" href="/" title="Home" class="nav-brand"><img src="http://placehold.it/50x20" alt=""></a>
            
            <!-- For right positioning use slot -->
            <li slot="right"><a href="/" target="_blank">Login</a></li>
            <li slot="right"><a href="/" target="_blank">Register</a></li>
               
            <li slot="right">
                <a href="/" target="_blank"><img src="http://placehold.it/20x20" alt=""></a>
            </li>
            <li slot="right">
                <a href="/" target="_blank"><img src="http://placehold.it/20x20" alt=""></a>
            </li>
            <li slot="right">
                <a href="/" target="_blank"><img src="http://placehold.it/20x20" alt=""></a>
            </li>
        </navbar>
        <div class="cover clearfix">
            
            <div class="col-xs-12 col-md-8 col-md-push-4 cover-image " style="background-image: url('https://d13yacurqjgara.cloudfront.net/users/1092767/screenshots/2983878/dribbble800x600.png')"></div>
            <div class="col-xs-12 col-md-4 col-md-pull-8 cover-info">
                
                <h2>กลุ่มทอเสื่อกก</h2>
                <h2>(นางกฤษณา ปะวะดี)</h2>
                <br>
                <br>
                <a href="/"><img class="round" src="http://placehold.it/50x50"></a>
                <p>Write the first review</p>
            </div>
        </div>
        <div class="detail container">
            <div class="col-xs-8 col-xs-offset-2">
                <div class="clearfix">
                    <div class="col-xs-6"><img class="round" src="http://placehold.it/50x50"><span class="click-able" @click="tab='description'">Description</span></div>
                    <div class="col-xs-6"><img class="round" src="http://placehold.it/50x50"><span class="click-able" @click="tab='review'">Review</span></div>
                </div>
                <div class="wall-of-text description" v-if="tab=='description'">
                    บอยคอต เวิลด์เที่ยงวันฟินิกซ์แตงกวาเบญจมบพิตร โดนัทออเดอร์หล่อฮังก้วย เดโมไชน่าเบิร์ด วอล์ก เซนเซอร์เรตติ้งบลูเบอร์รีไฟต์ 
                    ปาสคาล กลาสช็อตจูเนียร์เพียว อาร์ติสต์พาสปอร์ตติงต๊องวิว แชเชือนควิก เซี้ยวซิมโฟนี่ก่อนหน้าเบนโตะสปอร์ต 
                    แคมเปญรีดไถคาราโอเกะปาสคาล แมกกาซีนแอพพริคอทฟลอร์ อุรังคธาตุคอร์สบ๊อกซ์ คอนแท็คเปียโนพะเรอสะเด่า 
                    ฟรุตเวิลด์คอนเซปต์ไคลแม็กซ์อีสต์

                    ตี๋ภารตะแจ๊กพอต ไทยแลนด์ วอล์คติงต๊องโปสเตอร์ อาร์พีจีเมี่ยงคำแอดมิสชันลอจิสติกส์เกย์ เดบิตสตริง 
                    โปรโมชั่นอ่วมซัพพลาย อพาร์ตเมนต์แมคเคอเรลแคนยอนสตรอเบอร์รีแลนด์ บอกซ์วาซาบิซาร์ดีนยิวไมค์ โก๊ะเหมยพาเหรด 
                    แอโรบิคธัมโม วาไรตี้ ปาสกาลโยเกิร์ตศิลปวัฒนธรรม ยอมรับเรตติ้งผ้าห่มซามูไรคันยิ แอปเปิ้ลโพสต์ รวมมิตรฟอร์มฟลอร์ 
                    หมิงแพกเกจไลท์ฮอตดอก
                </div>
                <div class="wall-of-text review" v-if="tab=='review'">
                    บอยคอต เวิลด์เที่ยงวันฟินิกซ์แตงกวาเบญจมบพิตร โดนัทออเดอร์หล่อฮังก้วย เดโมไชน่าเบิร์ด วอล์ก เซนเซอร์เรตติ้งบลูเบอร์รีไฟต์ <br><br>
                    บอยคอต เวิลด์เที่ยงวันฟินิกซ์แตงกวาเบญจมบพิตร โดนัทออเดอร์หล่อฮังก้วย เดโมไชน่าเบิร์ด วอล์ก เซนเซอร์เรตติ้งบลูเบอร์รีไฟต์ <br><br>
                    บอยคอต เวิลด์เที่ยงวันฟินิกซ์แตงกวาเบญจมบพิตร โดนัทออเดอร์หล่อฮังก้วย เดโมไชน่าเบิร์ด วอล์ก เซนเซอร์เรตติ้งบลูเบอร์รีไฟต์ <br><br>
                    บอยคอต เวิลด์เที่ยงวันฟินิกซ์แตงกวาเบญจมบพิตร โดนัทออเดอร์หล่อฮังก้วย เดโมไชน่าเบิร์ด วอล์ก เซนเซอร์เรตติ้งบลูเบอร์รีไฟต์ <br><br>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.min.css'
import { navbar, dropdown } from 'vue-strap'
export default {
    components: {
        navbar, dropdown
    },
    data() {
        return {
            tab: 'description'
        }
    }
}
</script>
<style scope>
    
</style>
<style>
    html {
        height: 100%;
    }
    .navbar-collapse, .navbar-fixed-top .navbar-collapse  {
        max-height: 400px !important;
    }
    .nav-brand {
        float: right;
        height: 50px;
        padding: 15px 15px;
        font-size: 14px;
        line-height: 20px;
        position: absolute;
        left: 0;
        right: 0;
        margin: auto;
        width: 50px;
    }
    .cover {
        background-color: #f0f0f0;
        height: 300px;
    }
    
    .cover-image {
        height: 300px;
        background-size: cover;
        background-position: center;
    }
    .cover-info {
        height: 300px;
        padding-top: 40px;
        background-color: #f0f0f0;
    }
    .cover-info h2 {
        margin: 0;
    }
    @media screen and (max-width: 991px) {
        .cover {
            background-color: #f0f0f0;
            height: auto;
        }
        .cover-info {
            height: 270px;
            padding-top: 40px;
            background-color: #f0f0f0;
        }
    }
    .detail {
        padding-top: 20px;
    }
    .wall-of-text {
        padding-top: 20px;
        text-indent: 20px;
        text-align: left;
    }
    .round {
        border-radius: 50%;
    }
    .click-able {
        cursor: pointer;
        padding-left: 10px;
    }
    .click-able:hover {
        text-decoration: underline;
    }
body {
    padding-bottom: 50px;
}

#app {
    color: #2c3e50;
    font-family: Source Sans Pro, Helvetica, sans-serif;
    text-align: center;
}


.logo {
    width: 100px;
    height: 100px
}
</style>
