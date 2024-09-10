<template>
    


    <div id="Events" class="events-section"></div>
</template>

<script>
export default{
    mounted(){
        this.scrollToSection();
    },
    methods:{
        scrollToSection(){
            const hash = this.$route.hash;
            if (hash){
                const element = document.getElementById(hash.substr(1));
                if(element){
                    element.scrollIntoView({behavior: 'smooth'})
                }
            }
        }
    },
    watch:{
        '$route'(){
            this.scrollToSection();
        }
    }
}
</script>