# CSS-External
Applicable to HTML code
*{
    margin: 0;
    padding: 0;
    font-family: 'poppins';
    box-sizing: border-box;
}

:root{
    --body-color: #efefef;
    --nav-color: #1876f2;
    --bg-color: #fff;
}
.dark-theme{
    --body-color: #0a0a0a;
    --nav-color: #000;
    --bg-color: #000;
}



body{
    background: var(--body-color);
    transition: background 0.3s;
}
nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    background: var(--nav-color);
    padding: 5px 5%;
    position: sticky;
    top: 0;
    z-index: 100;
}
.logo{
    width: 160px;
    margin-right: 45px;
}
.nav-left, .nav-right{
    display: flex;
    align-items: center;
}
.nav-left ul li{
    list-style: none;
    display: inline-block;
}
.nav-left ul li img{
    width: 25px;
    margin: 0 20px;
}
.nav-user-icon img{
    width: 40px;
    border-radius: 50%;
    cursor: pointer;
}
.nav-user-icon{
    margin-left: 30px;
}

.search-box{
    background: #efefef;
    width: 350px;
    border-radius: 20px;
    display: flex;
    align-items: center;
    padding: 0 15px;
}
.search-box img{
    width: 20px;
}
.search-box input{
    width: 100%;
    background: transparent;
    padding: 10px;
    outline: none;
    border: 0;
}
.online{
    position: relative;
}
.online::after{
    content: '';
    width: 7px;
    height: 7px;
    border: 2px solid #fff;
    border-radius: 50%;
    background: #41db51;
    position: absolute;
    top: 0;
    right: 0;
}

.container{
    display: flex;
    justify-content: space-between;
    padding: 13px 5%;
}
.left-sidebar{
    flex-basis: 25%;
    position: sticky;
    top: 70px;
    align-self: flex-start;

}
.right-sidebar{
    flex-basis: 25%;
    position: sticky;
    top: 70px;
    align-self: flex-start;
    background: var(--bg-color);
    padding: 20px;
    border-radius: 4px;
    color: #626262;
}
.main-content{
    flex-basis: 47%;
}

.imp-links a, .shortcut-links a{
    text-decoration: none;
    display: flex;
    align-items: center;
    margin-bottom: 30px;
    color: #626262;
    width: fit-content;
}
.imp-links a img{
    width: 25px;
    margin-right: 15px;
}
.imp-links a:last-child{
    color: #1876f2;
}
.imp-links{
    border-bottom: 1px solid #ccc;
}
.shortcut-links a img{
    width: 40px;
    border-radius: 4px;
    margin-right: 15px;
}
.shortcut-links p{
    margin: 25px 0;
    color: #626262;
    font-weight: 500;
}

.sidebar-title{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 18px;
}
.right-sidebar h4{
    font-weight: 600;
    font-size: 16px;
}
.sidebar-title a{
    text-decoration: none;
    color: #1876f2;
    font-size: 12px;
}
.event{
    display: flex;
    font-size: 14px;
    margin-bottom: 20px;
}
.left-event{
    border-radius: 10px;
    height: 65px;
    width: 65px;
    margin-right: 15px;
    padding-top: 10px;
    text-align: center;
    position: relative;
    overflow: hidden;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
.event p{
    font-size: 12px;
}
.event a{
    font-size: 12px;
    text-decoration: none;
    color: #1876f2;
}
.left-event span{
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    background: #1876f2;
    color: #fff;
    font-size: 10px;
    padding: 4px 0;
}
.sidebar-ads{
    width: 100%;
    margin-bottom: 20px;
    border-radius: 4px;
}
.online-list{
    display: flex;
    align-items: center;
    margin-bottom: 20px;

}
.online-list .online img{
    width: 40px;
    border-radius: 50%;
}
.online-list .online{
    width: 40px;
    border-radius: 50%;
    margin-right: 15px;
}
.online-list .online::after{
    top: unset;
    bottom: 5px;
}


.story-gallery{
    display: flex;
    justify-content: space-between;
    margin-bottom: 20px;
}
.story{
    flex-basis: 18%;
    padding-top: 32%;
    position: relative;
    background-image: linear-gradient(transparent,rgba(0,0,0,0.5)),url(C:/Users/Dell/Desktop/images/status-1.png);
    background-position: center;
    background-size: cover;
    border-radius: 10px;
}
.story img{
    position: absolute;
    width: 45px;
    border-radius: 50%;
    top: 10px;
    left: 10px;
    border: 5px solid #1876f2;
}
.story p{
    position: absolute;
    bottom: 10px;
    width: 100%;
    text-align: center;
    color: #fff;
    font-size: 14px;    
}
.story1{
    background-image: linear-gradient(transparent,rgba(0,0,0,0.5)),url(C:/Users/Dell/Desktop/images/status-1.png);
}
.story2{
    background-image: linear-gradient(transparent,rgba(0,0,0,0.5)),url(C:/Users/Dell/Desktop/images/status-2.png);
}
.story3{
    background-image: linear-gradient(transparent,rgba(0,0,0,0.5)),url(C:/Users/Dell/Desktop/images/status-3.png);
}
.story4{
    background-image: linear-gradient(transparent,rgba(0,0,0,0.5)),url(C:/Users/Dell/Desktop/images/status-4.png);
}
.story5{
    background-image: linear-gradient(transparent,rgba(0,0,0,0.5)),url(C:/Users/Dell/Desktop/images/status-5.png);
}
.story.story1 img{
    top: unset;
    left: 50%;
    bottom: 40px;
    transform: translatex(-50%);
    border: 0;
    width: 35;
}
.write-post-container{
    width: 100%;
    background: var(--bg-color);
    border-radius: 6px;
    padding: 20px;
    color: #626262;
}
.user-profile{
    display: flex;
    align-items: center;
}
.user-profile img{
    width: 45px;
    border-radius: 50;
    margin-right: 10px;
}
.user-profile p{
    margin-bottom: -5px;
    font-weight:  500;
    color: #626262;
}
.user-profile small{
    font-size: 12px;
}
.post-input-container{
    padding-left: 55px;
    padding-top: 20px;
}
.post-input-container textarea{
    width: 100%;
    border: 0;
    outline: 0;
    border-bottom: 1px solid #ccc;
    background: transparent;
    resize: none;
}
.add-post-links{
    display: flex;
    margin-top: 10px;

}
.add-post-links a{
    text-decoration: none;
    display: flex;
    align-items: center;
    color: #626262;
    margin-right: 30px;
    font-size: 13px;
}
.add-post-links a img{
    width: 20px;
    margin-right: 10px;
}
.post-container{
    width: 100%;
    background: var(--bg-color);
    border-radius: 6px;
    padding: 20px;
    color: #626262;
    margin: 20px 0;
}
.user-profile span{
    font-size: 13px;
    color: #9a9a9a;
}
.post-text{
    color: #9a9a9a;
    margin: 15px 0;
    font-size: 15px;
}
.post-text span{
    color: #626262;
    font-weight: 500;
}
.post-text a{
    color: #1876f2;
    text-decoration: none;
}
.post-img{
    width: 100%;
    border-radius: 4px;
    margin-bottom: 5px;
}
.post-row{
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.activity-icons div img{
    width: 18px;
    margin-right: 10px;
}
.activity-icons div{
    display: inline-flex;
    align-items: center;
    margin-right: 30px;
}
.post-profile icon{
    display: flex;
    align-items: center;
}
.post-profile-icon img{
    width: 20px;
    border-radius: 50%;
    margin-right: 5px;
}
.post-row a{
    color:#9a9a9a;
}
.load-mode-btn{
    display: block;
    margin: auto;
    cursor: pointer;
    padding: 5px 10px;
    border: 1px solid #9a9a9a;
    color:#626262;
    background: transparent;
    border-radius: 4px;
}
.footer{
    text-align: center;
    color: #9a9a9a;
    padding: 10px 0 20px;
    font-size: 13px;
}
.settings-menu{
    position: absolute;
    width: 90%;
    max-width: 350px;
    background: var(--bg-color);
    box-shadow: 0 0 10px rgba(0,0,0,0.4);
    border-radius: 4px;
    overflow: hidden;
    top: 108%;
    right: 5%;
    max-height: 0;
    transition: max-height 0.3s;
}
.settings-menu-height{
    max-height: 450px;
}
.user-profile a{
    font-size: 12px;
    color: #1876f2;
    text-decoration: none;
}
.settings-menu-inner{
    padding: 20px;
}
.settings-menu hr{
    border: 0;
    height: 1px;
    background: #9a9a9a;
    margin: 15px 0;
}
.settings-links{
    display: flex;
    align-items: center;
    margin: 15px 0;
}
.settings-links .settings-icon{
    width: 38px;
    margin-right: 10px;
    border-radius: 50%;
}
.settings-links a{
    display: flex;
    flex: 1;
    align-items: center;
    justify-content: space-between;
    text-decoration: none;
    color: #626262;
}
#dark-btn{
    position: absolute;
    top: 20px;
    right: 20px;
    background: #ccc;
    width: 45px;
    border-radius: 15px;
    padding: 2px 3px;
    cursor: pointer;
    display: flex;
    transition: padding-left 0.5s, backround 0.5s;
}
#dark-btn span{
    width: 18px;
    height: 18px;
    background: #fff;
    border-radius: 50%;
    display: inline-block;
}
#dark-btn.dark-btn-on{
    padding-left: 23px;
    background: #0a0a0a;
}
