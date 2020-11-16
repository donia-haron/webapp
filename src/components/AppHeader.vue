<template>


    <div class="header">

      
        <div class="container">
            <div class="logo1">
                <a href="#">

                    <img src="../assets/logoweb2.jpg" width="120px" alt="">
                    <h1 class="spn1" style="color:#C71585">Vote To Buy</h1>

                </a>   <div class="container h-100">
                    <div class="d-flex justify-content-center h-100">
                        <div class="searchbar">
                            <input class="search_input" type="text" name="" placeholder="Search...">
                            <a href="#" class="search_icon"><i><font-awesome-icon :icon="['fas', 'search']" /></i></a>
                        </div>
                    </div>
                </div>



            

            </div> 

                    <ul class="text-right">
                        <router-link to="/" tag="li" exact>
                            <a><i><font-awesome-icon :icon="['fas', 'home']" /></i></a>
                        </router-link> |
                        <router-link to="/blog" tag="li">
                            <a><i ><font-awesome-icon :icon="['fas', 'female']" /></i></a>
                        </router-link> |
                        <router-link to="/about" tag="li">
                            <a><i><font-awesome-icon :icon="['fas', 'user']" /></i></a>
                        </router-link> |
                        <router-link to="/help" tag="li" >
                            <a><i><font-awesome-icon :icon="['fas', 'shopping-cart']" /></i></a>
                        </router-link>

                    </ul>
                </div>
            </div>
    </template>
    <script>
        export default{
        name:'AppHeader'

        };
    </script>

    <style lang="scss" scoped>
        .searchbar {
            margin-bottom: auto;
            margin-top: auto;
            height: 60px;
            background-color: #353b48;
            border-radius: 30px;
            padding: 10px;
        }

        .search_input {
            color: white;
            border: 0;
            outline: 0;
            background: none;
            width: 0;
            caret-color: transparent;
            line-height: 40px;
            transition: width 0.4s linear;
        }

        .searchbar:hover > .search_input {
            padding: 0 10px;
            width: 450px;
            caret-color: red;
            transition: width 0.4s linear;
        }

        .searchbar:hover > .search_icon {
            background: white;
            color: #e74c3c;
        }

        .search_icon {
            height: 40px;
            width: 40px;
            float: right;
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 50%;
            color: white;
            text-decoration: none;
        }
        ul li a i {
          font-size:30px; 
        
        }
        .header {
            background-color: #fadcda;
            background-repeat: no-repeat;
            background-size: cover;
            color: #ffff00;
            overflow: hidden;
            ul{
             float:left;
             width:calc(100% - 200px);

             li{margin:0;
                   display:inline-block;
                   padding:20px;
               a
        {
            color: #000 ;
            text-decoration: none;
        }
     
                   }
         }

         }
        .container{
            display:flex;

        }
        .container ul {
            padding-top:30px;
            font-size:20px;
        }
        .container .logo1{
            display:flex;
            width:500px;

            flex-direction:row;
        }
            .container .logo1 a:hover{
                text-decoration:none;
            }
            .container .logo1 a{
                display:flex;
            }
                .container .logo1 a h1{
                    padding-top:30px;
                    font-size:25px;
                    font-weight:bold;
                }
                .container .logo1 h1 {
                    font-size: 25px;
                    background: -webkit-linear-gradient( #ffff00,#C71585);
                    -webkit-background-clip: text;
                    -webkit-text-fill-color: transparent;
                }
     




    </style>
