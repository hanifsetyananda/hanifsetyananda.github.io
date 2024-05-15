<template>
    <section class="h-screen bg-black text-white">
        <div class="container mx-auto">
            <div class="flex justify-center mb-10"> 
            <span class="text-6xl text-center">SKILLS</span>
            </div>
            <div class="grid grid-cols-3 grid-flow-row gap-9" >
                <div class="" v-for="data in datas" v-if="datas">
                    <div class="grid grid-cols-1 p-4">
                        <span class="text-2xl mb-4"> {{data.title}}</span>
                        <span>{{data.description}}</span>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default{
        data(){
            return{
                datas : [
                    {
                        title : "Laravel",
                        description : "I Have 4 years of experience in laravel. Have a good understanding about OOP and Test Case"
                    }, 
                    {
                        title : "Laravel",
                        description : "I Have 4 years of experience in laravel. Have a good understanding about OOP and Test Case"
                    }, 
                    {
                        title : "Laravel",
                        description : "I Have 4 years of experience in laravel. Have a good understanding about OOP and Test Case"
                    }, 
                ],

            }
        }
    }

</script>
