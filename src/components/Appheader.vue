<script>
export default{
    data(){
        return{
            sessi:[
                {
                    gender: 'Donna'
                },
                {
                    gender: 'Uomo'
                },
                {
                    gender: 'Bambino'
                }
            ],

            icons:[
                {
                    iconName: 'fa-regular fa-user'
                },
                {
                    iconName: 'fa-regular fa-heart'
                },
                {
                    iconName: 'fa-solid fa-cart-shopping'
                }
            ],
        };
    },
};
</script>

<template>
    <nav>
        <div class="nav-container">
            <div class="sesso">
                <span v-for="sesso in sessi" class="gender">{{ sesso.gender }}</span>
            </div>
                <div class="logo-container"><img src="../assets/img/boolean-logo.png" alt="logo"></div>
                    <div class="account">
                        <i v-for="icon in icons" :class="icon.iconName"></i>
                    </div>
                </div>
    </nav>
</template>

<style lang="scss">
nav{
    .nav-container{
    display: flex;
    justify-content: center;
    height: 40px;
    background-color: #FF6900;
    box-shadow: 0px 1px 3px 2px rgba(0,0,0,0.43);
    color: white;
    position: sticky;
    top: 0;

    .sesso{
    text-align: start;
    width: 400px;
    min-width: 200px;
    line-height: 40px;

        .gender{
            margin-right: 5px;
        }
    }

    .logo-container{
    text-align: center;
    width: 150px;
    min-width: 100px;
    padding: 4px;

        img{
        width: 150px;
        line-height: 40px;
        min-width: 100px;
        }
    }

    .account{
    text-align: end;
    width: 400px;
     min-width: 200px;
     line-height: 40px;

        .fa-regular.fa-user,
        .fa-regular.fa-heart{
            margin-right: 5px;
        }
    }
}
}
</style>
