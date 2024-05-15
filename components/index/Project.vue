<template>
    <section class="h-screen bg-black text-white"> 
        <div class="container mx-auto">
            <div class="flex justify-center mb-10"> 
                <span class="text-6xl text-center">PROJECTS</span>
            </div>
            <div class="grid grid-cols-1">
                <table class="table-auto border-t-2">
                    <tr v-for="tbl in tableData">
                        <td class="border-r-2">
                            <div class="grid grid-cols-1 object-top">
                                <span>{{tbl.name}}</span>
                                <span>{{tbl.number}}</span>
                            </div>


                        </td>

                        <td class="border-r-2 p-5"><img :src="tbl.images" class="object-center mx-auto w-[864px] h-[486px]" /></td>
                        <td>
                            <div class="grid grid-cols-1">
                                <span>YEAR</span>
                                <span>{{tbl.year}}</span>
                                <span>ROLE</span>
                                <span>{{tbl.role}}</span>
                                <span>TECHS</span>
                                <div>
                                    <span v-for="tech in tbl.techs">{{tech}}</span>
                                </div>
                                <span>{{tbl.description}}</span>
                            </div>
                        </td>
                    </tr>
                </table>
            </div>
        </div>
    </section>
</template>

<script>
    export default{
        data(){
            return {
                tableData : [
                    {
                        number: "01",
                        name:"Project Name",
                        images:"https://dummyimage.com/864x486/fff/000",
                        year:"2024",
                        role:"Backend Engineer",
                        techs:["PHP","Javascript","Kotlin"],
                        description:"Lorem ipsum dolor et si labor"
                    }
                ]
            }
        }
    }
</script>
