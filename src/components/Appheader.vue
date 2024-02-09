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

</style>
