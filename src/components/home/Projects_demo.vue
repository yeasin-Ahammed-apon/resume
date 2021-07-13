<template>
  <section  id="projects">
      <h2 class="m-5">Projects</h2> 
      <div class="row justify-content-center">            
            <div class="card col-md-3 col-sm-12 m-1" v-for="project in projects" :key="project.id">
                <div class="card-body">
                    <h5 class="card-title">{{project.name}}</h5>                                        
                    <a :href="project.github" class="btn btn-dark"><i class="fab fa-github"></i></a>                    
                    <span v-if='project.youtube==null'>
                        <!-- noting to show if youtube is null  -->
                    </span>                    
                    <span v-else>
                        <a :href="project.youtube" class="btn btn-danger m-1"><i class="fab fa-youtube "></i></a>                    
                    </span>
                         <a :href="project.readmore" class="btn btn-primary ms-1"><i class="fab fa-readme"></i></a>                                                            
                </div>
            </div>
      </div>            
  </section>
</template>

<script>
export default {
    data() {
        return {
            projects:[
		{
                    id:8,
                    name:"e-commerce_cart-system_SPA_use-of-localstorage-CRUD_vue2_vuex_vue-router",
                    github:"https://github.com/yeasin-Ahammed-apon/e-commerce_cart-system_SPA_use-of-localstorage-CRUD_vue2_vuex_vue-router",                    
                    readmore:"https://github.com/yeasin-Ahammed-apon/e-commerce_cart-system_SPA_use-of-localstorage-CRUD_vue2_vuex_vue-router/blob/main/README.md",
                    youtube:null
                },
                {
                    id:7,
                    name:"vue_todoList_with_localStorage",
                    github:"https://github.com/yeasin-Ahammed-apon/vue_todoList_with_localStorage",                    
                    readmore:"https://github.com/yeasin-Ahammed-apon/vue_todoList_with_localStorage/blob/main/README.md",
                    youtube:null
                },
                {
                    id:6,
                    name:"laravel_loging_reg_edit_profile_and_edit_data",
                    github:"https://github.com/yeasin-Ahammed-apon/laravel_loging_reg_edit_profile_and_edit_data",                    
                    readmore:"https://github.com/yeasin-Ahammed-apon/laravel_loging_reg_edit_profile_and_edit_data/blob/main/README.md",
                    youtube:null
                },
                {
                    id:5,
                    name:"laravel_middleware_and_auth",
                    github:"https://github.com/yeasin-Ahammed-apon/laravel_middleware_and_auth",
                    readmore:"https://github.com/yeasin-Ahammed-apon/laravel_middleware_and_auth/blob/main/README.md",
                    youtube:null
                },
                {
                    id:4,
                    name:"pdf_crud",
                    github:"https://github.com/yeasin-Ahammed-apon/pdf_crud",
                    readmore:"https://github.com/yeasin-Ahammed-apon/pdf_crud/blob/main/README.md",
                    youtube:null
                },
                {
                    id:3,
                    name:"image_crud",
                    github:"https://github.com/yeasin-Ahammed-apon/image_crud",
                    readmore:"https://github.com/yeasin-Ahammed-apon/image_crud/blob/main/README.md",
                    youtube:null
                },
                 {
                    id:2,
                    name:"laravel_RDBMS_relational_database_management_system",
                    github:"https://github.com/yeasin-Ahammed-apon/laravel_RDBMS_relational_database_management_system",
                    readmore:"https://github.com/yeasin-Ahammed-apon/laravel_RDBMS_relational_database_management_system/blob/main/README.md",
                    youtube:null
                },
                {
                    id:1,
                    name:"simple_blog_project",
                    github:"https://github.com/yeasin-Ahammed-apon/simple_blog_project",
                    readmore:"https://github.com/yeasin-Ahammed-apon/simple_blog_project/blob/main/README.md",
                    youtube:null
                },
                
            ]
        };
    },

}
</script>

<style>

</style>