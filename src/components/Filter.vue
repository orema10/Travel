<template>
    <section class="filter">
        <div class="filter-container">
            <input class="search" placeholder="Search ..." type="text" />
            <countries></countries>
            <citys></citys>
            <button>Filter</button>
        </div>
    </section>
</template>

<script>
import countries from './Countries';
import citys from './Citys';
export default {
    components: {
        countries,
        citys
    }
}
</script>

<style scoped>
section.filter {
    position: fixed;
    left: 0;
    width: 15vw;
    height: 100vh;
    /* background-color: lightgray; */
}

section.filter .filter-container {
    width: 80%;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 100%;
    justify-content: space-around;
}

section.filter .filter-container input {
    background: url('../assets/img/icons/MagnifyingGlass.svg');
    background-repeat: no-repeat;
    background-size: 15px 15px;
    background-position: left;
    padding-left: 20px;
    padding-bottom: 3px;
    border-bottom: 1px solid rgba(0,0,0,0.4);
}

section.filter .filter-container input::placeholder {
    color: #333;
    opacity: .7;
    letter-spacing: .5px;
}

section.filter .filter-container input:-ms-input-placeholder {
    color: #333;
    opacity: .7;
    letter-spacing: .5px;
}

section.filter .filter-container input::-ms-input-placeholder {
    color: #333;
    opacity: .7;
    letter-spacing: .5px;
}

</style>
