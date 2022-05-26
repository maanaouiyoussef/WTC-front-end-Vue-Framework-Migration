<template>
    <!-- Navbar -->
    <nav id="main-h-nav" class="">
        <ul class="nav-item-container">
            <li class="nav-item">
                <a href="#" class="nav-link active">Content Live Audit</a>
            </li>
            <li class="nav-item">
                <a href="#" class="nav-link">Child Level Scoring View</a>
            </li>
            <li class="nav-item">
                <a href="#" class="nav-link">Parent Scoring View</a>
            </li>
            <li class="nav-item">
                <a href="#" class="nav-link">Audit Details</a>
            </li>
            <li class="nav-item">
                <a href="#" class="nav-link">A+ Control </a>
            </li>
            <li class="nav-item">
                <a href="#" class="nav-link">Reviews Overview</a>
            </li>
            <li class="nav-item">
                <a href="#" class="nav-link">Q&As</a>
            </li>
        </ul>
    </nav>
    <!-- Navbar End -->
</template>

<script>
export default {
    name: 'NavBar',
    components: {

    }
}
</script>


<style scoped>
/* Navbar */
#main-h-nav {
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px;
    font-size: 13pt;
    border-bottom: 1px solid #f2f2f2;
}

.nav-item {
    display: inline-block;
    padding: 0 20px;
}

.nav-link {
    color: #4d4f5c;
}

.nav-link.active {
    color: #0946ec;
    background-color: #f2f2f2;
    padding: 8px;
    text-decoration: underline;
    font-weight: bold;
}
</style>