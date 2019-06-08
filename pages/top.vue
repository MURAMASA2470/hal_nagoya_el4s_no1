<template>
    <div>

    <div class="image">
        <v-img src="https://cdn.discordapp.com/attachments/529305618624938004/586722619802255390/13x.png" height="92.35vh" width="100vw"></v-img>
    </div>
    
    <div class="btn">
        <nuxt-link to="/create" style="color: white;text-decoration: none;"><v-btn color="#2FCB71">OsuTabiを始める</v-btn></nuxt-link>
        <v-btn outline color="#2FCB71">ログインする</v-btn>
    </div>

    </div>
</template>

<style>
    .v-footer {
        display: none;
    }
</style>

<style scoped>
    .image {
        position: absolute;
        top: 0;
        left: 0;
    }
    .btn {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100vw;
    }

        .btn button {
            width: 80%;
            height: 60px;
            margin: 20px 40px;
        }

        .v-btn--outline {
            background-color: black !important; 
            opacity: 0.5;
            color: white !important;
            border-color: #2FCB71;
        }
        
</style>

