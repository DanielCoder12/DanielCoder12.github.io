<template>
    <div class=" col-10 p-4 d-none d-md-block">
        <p class="fw-bold">My Skills</p>
        <div class="justify-content-between fs-4 d-flex">
            <span class="skill" v-for="skill in skills" :key="skill">{{ skill }}</span>
        </div>
    </div>
    <div class="d-inline bg d-md-none">

        <p class="fw-bold">My Skills</p>
        <!-- <div class="d-flex"> -->
        <p class="" v-for="skill in skills" :key="skill"> {{ skill }}</p>
        <!-- </div> -->

    </div>
</template>


<script>
import { AppState } from '../AppState';
import { computed, reactive, onMounted } from 'vue';
export default {
    setup() {
        let skills = ['HTML', 'CSS', 'JS', 'C#', 'VUE', 'SQL', '.NET', 'Node.js']
        return {
            skills
        }
    }
};
</script>


<style lang="scss" scoped>
.skill {
    background-color: pink;
    border-radius: 50%;
    height: 5.5rem;
    aspect-ratio: 1/1;
    align-items: center;
    display: flex;
    justify-content: center;
}

.bg {
    background-color: pink;
}
</style>