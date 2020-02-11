<template>
    <Page>
        <ActionBar>
            <Label text="Home"></Label>
        </ActionBar>
        
        <FlexboxLayout flexDirection="column">
          <label text="First Text" height="70" backgroundColor="#43b883"/>
          <label text="Second" height="70" backgroundColor="#1c6b48"/>
          <label text="Third" height="70" backgroundColor="#289062"/>
        </FlexboxLayout>
        
        <!-- <ActionBar>
            <StackLayout orientation="horizontal">
                <Image src="res://icon" width="40" height="40" verticalAlignment="center" />
                <Label text="NativeScript" fontSize="24" verticalAlignment="center" />
            </StackLayout>
       </ActionBar> -->
    </Page>
</template>

<script>
    export default {
        computed: {
            message() {
                return "Hello Omair";
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
