<template>
    <Page>
        <ActionBar>
            <Label text="Home"></Label>
            <NavigationButton text="back" android.systemIcon="ic_menu_back" @tap="goBack" />
        </ActionBar>
        
       
       
    </Page>
</template>

<script>
    export default {
        computed: {
            message() {
                return "Hello Omair";
            }
        },
        data(){
            return{
                selectedDate:'4/2/1996'       
            }
        }
    };
</script>

<style scoped lang="scss">
    @import '~@nativescript/theme/scss/variables/blue';
FlexboxLayout{
    margin-top: 2rem;
}    
</style>
