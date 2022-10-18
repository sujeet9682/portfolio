* {
    margin: 0;
    padding: 0;
    font-family: Arial, Helvetica, sans-serif;
    box-sizing: border-box;
}

body {
    background: #080808;
    color: #fff;
}

html{
    scroll-behavior: smooth;
}
#header {
    width: 100%;
    height: 100vh;
    background-image: url(1.jpg);
    background-size: cover;
    background-position: center;
}

.container {
    padding: 10px 10px;
}
.navb{
    background:black;

}

nav {
    display: flex;
    position: fixed;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
   
}

.bars{
    list-style: none;
}

.logo {
    width: 140px;
    text-decoration: none;
    list-style: none;
    color: bisque;
    font-size: medium;
    margin: 10px;
    padding: 20px 3px;
    font-size: 25px;
}

.bttn{
    text-decoration:dotted;
    color: greenyellow;
}
.btm{
    margin: 10px 10px;
    background-color:rgb(58, 8, 152);
    border-radius: 7px;
}

nav ul li {
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
    
}



nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
    position: relative;
}

nav ul li a::after {
    content: '';
    width: 0;
    height: 3px;
    background: red;
    position: absolute;
    left: 0;
    bottom: -6px;
    transition: 0.2s;
}

nav ul li a:hover::after {
    width: 100%;
}

.aboutp {
    margin-top: 200px;
    margin-left: 90px;
}

.header-text h1 {
    font-size: 60px;
    margin-top: 20px;
    margin-left: 90px;
}

.header-text span {
    color: #ff04ff;
}

/*  ---------About------------ */

#about {
    padding: 88px 0;
    color: antiquewhite;
}

.row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.about-col-1 {
    flex-basis: 35%;
}

.about-col-1 img {
    width: 100%;
    border-radius: 15px;
}

.about-col-2 {
    flex-basis: 60%;
}

.sub-title {
    font-size: 60px;
    font-weight: 600;
    color: #fff;
}

.tab-titles {
    display: flex;
    margin: 20px 0 40px;
}

.tab-links {
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    cursor: pointer;
    position: relative;
}

.tab-links::after {
    content: '';
    width: 0;
    height: 3px;
    background: #ff04ff;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
}

.tab-links.active-link::after {
    width: 50%;
}

.tab-contents ul li {
    list-style: none;
    margin: 10px 0;
}

.tab-contents ul li span {
    color: red;
    font-size: 14px;
}

.tab-contents {
    display: none;
}

.tab-contents.active-tab {
    display: block;
}

/* -------------------services----------- */

#services {
    padding: 30px 0;
}

.services-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}

.services-list div {
    background: #262626;
    padding: 40px;
    font-size: 13px;
    font-weight: 300;
    border-right: 10px;
    border-radius: 10px;
    transition: background 0.5s, transform 0.5s;
}

.services-list div i {
    font-size: 50px;
    margin-bottom: 30px;
}

.services-list div h2 {
    font-size: 30px;
    font-weight: 500;
    margin-bottom: 14px;
}

.services-list div a {
    text-decoration: none;
    color: #fff;
    font-size: 12px;
    margin-top: 20px;
    display: inline-block;
}

.services-list div:hover {
    background-color: #ff004f;
    transform: translateY(10px);
}

.work-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}

.work{
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}

.work img{
    width: 100%;
    border-radius: 10px;
    display: block;
    transition: transform 0.5s;
}

.layer{
    width: 100%;
    height: 100%;
    background: linear-gradient(rgba(0,0,0,0.6), #ff004f);
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 40px;
    text-align: center;
    transition: height 0.5s;
}

.layer h3{
    font-weight: 500;
    margin-bottom: 20px;
}

.work:hover img{
    transform: scale(1.1);
}

.work:hover layer{
    height: 100%;
}

.copyright{
    width: 100%;
    text-align: center;
    padding: 25px 0;
    background: #262626;
    font-weight: 300;
    margin-top: 33px;
}

.thanks {
    font-size: 60px;
    font-weight: 600;
    color: #fff;
    text-align: center;
}

.bars{
    display: none;
}
@media screen and (max-width: 600px){
    #header{
        background-image: url(2.jpg);
    }
    .header-text{
        margin-top: 100%;
        font-size: 16px;
    }
    .header-text h1{
        font-size: 30px;
    }

    .bars{
        display: block;
        font-size: 1ki5px;
    }
    nav ul{
        background: #ff004f;
        position: fixed;
        top: 0;
        right: -200px;
        width: 200px;
        height: 100vh;
        padding-top: 50px;
        z-index: 2;
    }
    nav ul li{
        display: block;
        margin: 25px;
    }
    .sub-title{
        font-size: 40px;
    }
    .about-col-1, .about-col-2{
        flex-basis: 100%;
    }
    .about-col-1{
        margin-bottom: 30px;
    }
    .about-col-2{
        font-size: 14px;
    }
    .tab-links{
        font-size: 16px;
        margin-right: 20px;
    }
    .copyright{
        font-size: 14px;
    }
}
