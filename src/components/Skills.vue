<script>
export default {
    data() {
        return {
            skills: [
                { title: 'C/C++', id: 1, details: "I have written my first lines of code in C language and that was a start of a beautiful journey. Also, I have used a little bit of C++ when learning about Algorithms and Data Structures."},
                { title: 'Java', id: 2, details: "I can't say I know a lot of Java, but it was the language I used when I was learning and using object oriented concepts for the first time."},
                { title: 'HTML & CSS', id: 3, details: "Foundation of every web site. When I first learned basics of HTML and CSS in highschool, I couldn't believe that web world was that \"simple\". I still can't believe how much stuff you can build using only those two."},
                { title: 'Bootstrap', id: 4, details: "Talking about CSS, Bootstrap is a very easy and powerful CSS component framework I have used. Also, I am familiar with utility frameworks such as Tailwind, but didn't use it as much."},
                { title: 'JavaScript', id: 5, details: "I rembember several years ago I wondered what was the difference beetween Java and JavaScript. Luckily, today I know that JavaScript is a script language and one skill you can't live without if you are working in web development. I always stick to it, but I would love to learn TypeScript also."},
                { title: 'Vue.js', id: 6, details: "Really great front end framework which I enjoyed using while making a single page web application."},
                { title: 'Node.js', id: 7, details: "My first steps in the world of back end development. I haven't really used it that much, only for laboratory excercises at university."},
                { title: 'PostgreSQL', id: 8, details: "Very simple tool for managing databases. I don't have that much experience in it, but I used it in some occasions."},
                { title: 'Visual Studio Code', id: 9, details: "Nothing much to say here. For me, and I believe for many developers out there, definetly an IDE of choice. Plugins make your coding experience much more enjoyable."},
                { title: 'Git', id: 10, details: "Very important system in the world of software developing. One year ago I thought terms \"push\" and \"pull\" very only used in gym and fitness scenarios, and that you have to \"commit\" when you are in a relationship... Little did I know, I would use those terms very frequently in a very different environment."}
            ]
        }
    }
}


</script>

<template>

<div class="d-flex justify-content-center align-items-center mt-3">
    <div class="badge bg-dark text-wrap text-white ms-2">
        <h1>Technologies & Skills</h1>
    </div>
</div>

<div class="container">
    <div class="row">
        <div class="col-md-12">
            <div class="accordion mt-3" id="accordionExample" v-for="skill in skills" :key="skill.id">
                <div class="accordion-item">
                    <h2 class="accordion-header" id="headingOne">
                        <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                        {{skill.title}}
                        </button>
                    </h2>
                    <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordionExample">
                        <div class="accordion-body">
                        {{skill.details}}
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

  

</template>