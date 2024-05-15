<template>
    <section class="h-screen bg-black text-white"> 
        <div class="container mx-auto">
            <div class="flex justify-center mb-10"> 
                <span class="text-6xl text-center">PROJECTS</span>
            </div>
            <div class="grid grid-cols-1">
                <table class="table">
                    <tr v-for="tbl in tableData">
                        <td>{{tbl.name}}</td>
                        <td><img :src="tbl.images" /></td>
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
                        name:"Project Name",
                        images:"",
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
