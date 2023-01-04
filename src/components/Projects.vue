<script>
export default {
    data() {
        return {
            projects: [
                { title: 'Minimal portfolio website', id: 1, description: "I have always wanted to make a web site that would represent me and my work to the world. Breaking the boring concept of CVs in a PDF file always seemed like a good idea. Also, I think it is a good practice for my first project." },
                { title: 'Forum for students', id: 2, description: "This was a group project we got assigned at university. It taught me how web applications are made from scratch. I also learned a lot about documentation behind the code of a product and what it means to deploy an application. I worked in the frontend department. Technologies we used were Vue.js and Bootstrap for CSS styling." }
            ]
        }
    }
}
</script>

<template>

<div class="d-flex justify-content-center align-items-center mt-3">
    <div class="badge bg-dark text-wrap ms-2">
        <h1>Projects</h1>
    </div>
</div>

<div class="container">
    
    <div class="row mt-3">

        <div class="col-md-6 d-flex mt-2" v-for="project in projects" :key="project.id">
            <div class="border border-3 rounded-top border-secondary bg-white">
                <div class="d-flex justify-content-center align-items-center border border-secondary bg-dark text-white">
                    <h3 class="text-uppercase">{{ project.title }}</h3>
                </div>
                <p class="m-2">
                    {{ project.description }}
                </p>
            </div>
        </div>
    </div>
</div>



<p class="text-center fw-bold lead mt-2">I hope to expand this area in the future!</p>

</template>