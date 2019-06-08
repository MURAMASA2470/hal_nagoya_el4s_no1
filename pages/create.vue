<template>
    <div class="wrap">

    <v-text-field
            label="メールアドレス"
            outline
          ></v-text-field>


    <v-text-field
            label="パスワード"
            outline
          ></v-text-field>


    <v-text-field
            label="ユーザー名"
            outline
          ></v-text-field>


    <v-select
          :items="items"
          label="出身国"
          :item="items"
          outline
        ></v-select>

        <div class="text-xs-center">
            <a href="/preview" style="text-decoration: none;"><v-btn round color="#2FCB71" style="width:85vw;height:60px;color:white;">登録する</v-btn></a>
        </div>
    </div>
    
</template>

<style scoped>
    .wrap {
        padding: 30px;
    }
</style>

<script>
export default {
    data: () => {
        return {
            items: [
                '日本', 'アメリカ', '中国', '韓国', '北朝鮮', 'イギリス', 'フランス', 'カンボジア'
            ]
        }
    }
}
</script>
