<template>
    <Page>
        <ActionBar>
            <Label text="Home"></Label>
            <NavigationButton text="back" android.systemIcon="ic_menu_back" @tap="goBack" />
        </ActionBar>
        
        <FlexboxLayout flexDirection="column">
          <label text="First" height="70" backgroundColor="#43b883"/>
          <label text="Second" height="70" backgroundColor="#1c6b48"/>
          <label text="Third" height="70" backgroundColor="#289062"/>
        </FlexboxLayout>
        
        <StackLayout>
            <Button text="Button" @tap="onButtonTap" />
        <Button>
            <FormattedString>
                <Span text="This text has a " />
                <Span text="red " style="color: red" />
                <Span text="piece of text. " />
                <Span text="Also, this bit is italic, " fontStyle="italic" />
                <Span text="and this bit is bold." fontWeight="bold" />
            </FormattedString>
            </Button>

        <DatePicker v-model="selectedDate"/>
        <Image src="https://art.nativescript-vue.org/NativeScript-Vue-White-Green.png" stretch="none" horizontalAlignment="center"/>    
        <!-- <ListPicker :items="listOfItems" v-model="selectedItem" /> -->
        <!-- <ListView for="item in listOfItems" @itemTap="onItemTap">
        <v-template>
            <Label :text="item.text" />
        </v-template>
        </ListView> -->
        <Progress :value="75" maxvalue="100"/>
        </StackLayout>
       
        <!-- <ActivityIndicator busy="true" @busyChange="onBusyChanged"/> -->
       
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
